# Implementing SPRINT collective variables

SPRINT collective variables were developed by Fabio Pietrucci and Wanda Andreoni and introduced in this paper in 2011.
I implemented them in PLUMED shortly after.  I don't think many people have found a use for these variables so there is no 
pressing need to develop a very fast implementation of these CVs.  I think a better approach is thus to implement these variables
in a way that helps potential future users understand what was done in Peitrucci and Andreoni's original paper.  For this reason,
the action SPRINT is implemented as a shortcut.  This means calculating and printing the SPRINT CVs is straightforward.  You 
just use the following input file:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_this_input_should_work.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="this_input_should_work.dats1" onclick='showPath("this_input_should_work.dat","this_input_should_work.dats1")'>s1</b>: <div class="tooltip" style="color:green">SPRINT<div class="right">Calculate SPRINT topological variables from an adjacency matrix. <a href="https://www.plumed.org/doc-master/user-doc/html/_s_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> GROUP1=1-7 SWITCH11={RATIONAL R_0=2.6 NN=6 MM=12}   
<span style="display:none;" id="this_input_should_work.dats1">The SPRINT action with label <b>s1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">s1.coord</td><td>all $n$ sprint coordinates are calculated and then stored in increasing order</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="this_input_should_work.dats1">s1</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

When PLUMED reads this it creates the more complicated input file shown below for calculating the SPRINT CVs.

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_this_input_should_work.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue"># Calculate a contact matrix that tells us about the bond between these 7 atoms</span>
<b name="this_input_should_work.dats1_mat" onclick='showPath("this_input_should_work.dat","this_input_should_work.dats1_mat")'>s1_mat</b>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUP=1-7 <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous switching function defined above<i></i></div></div>={RATIONAL R_0=2.6 NN=6 MM=12} 
<span style="color:blue"># Calculate the principle eigenvalue of the contact matrix and its corresponding eigenvector</span>
<span style="display:none;" id="this_input_should_work.dats1_mat">The CONTACT_MATRIX action with label <b>s1_mat</b> calculates a scalar quantity</span><b name="this_input_should_work.dats1_diag" onclick='showPath("this_input_should_work.dat","this_input_should_work.dats1_diag")'>s1_diag</b>: <div class="tooltip" style="color:green">DIAGONALIZE<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ARG=<b name="this_input_should_work.dats1_mat">s1_mat</b> VEC=1
<span style="color:blue"># Scale the eigenvector by multiplying it by the square root of the number of atoms and the corresponding eigenvalue </span>
<b name="this_input_should_work.dats1_sp" onclick='showPath("this_input_should_work.dat","this_input_should_work.dats1_sp")'>s1_sp</b>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=d1_diag.vals-1,<b name="this_input_should_work.dats1_diag">s1_diag.vecs-1</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=sqrt(7)*x*y <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<span style="color:blue"># Sort the compnents of scaled eigenvector </span>
<span style="display:none;" id="this_input_should_work.dats1_sp">The CUSTOM action with label <b>s1_sp</b> calculates a scalar quantity</span><b name="this_input_should_work.dats1" onclick='showPath("this_input_should_work.dat","this_input_should_work.dats1")'>s1</b>: <div class="tooltip" style="color:green">SORT<div class="right">This function can be used to sort colvars according to their magnitudes. <a href="https://www.plumed.org/doc-master/user-doc/html/_s_o_r_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="this_input_should_work.dats1_sp">s1_sp</b>
<span style="display:none;" id="this_input_should_work.dats1">The SORT action with label <b>s1</b> calculates a scalar quantity</span></pre>
 {% endraw %} 

A user looking in the log for PLUMED can thus see the individual steps involved in calculating this CV. In other words,
they can use PLUMED to get a sense of how these legacy CVs are calculated.  In fact, if you look at the first example input
above you should see the option to expand the shortcut in the tooltip that appears when you hover above SPRINT.  If you click
on this option something similar to the second input above appears.  Users thus do not even need to look in the log to see how 
these complicated CVs are calculated.  They can instead look through examples where such CVs have been used in the manual, tutorials 
and nest and use this option to expand shortcuts.

To get a sense of just how much PLUMED input can be hidden in these short inputs consider the following input for calculating 
SPRINT coordinates:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_this_input_should_work.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="this_input_should_work.datss" onclick='showPath("this_input_should_work.dat","this_input_should_work.datss")'>ss</b>: <div class="tooltip" style="color:green">SPRINT<div class="right">Calculate SPRINT topological variables from an adjacency matrix. <a href="https://www.plumed.org/doc-master/user-doc/html/_s_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> ...
   GROUP1=1-7 GROUP2=8-14 
   SWITCH11={RATIONAL R_0=2.6 NN=6 MM=12}
   SWITCH12={RATIONAL R_0=2.2 NN=6 MM=12}
   SWITCH22={RATIONAL R_0=2.2 NN=6 MM=12}
...
<span style="display:none;" id="this_input_should_work.datss">The SPRINT action with label <b>ss</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ss.coord</td><td>all $n$ sprint coordinates are calculated and then stored in increasing order</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=ss1.*,ss2 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

In this atom there are two distinct types of atom (A and B).  We thus have three different switching functions for describing 
whether the AA, AB and BB bonds.  If you look at the expanded version of the input above by clicking on the expand shortcut option
for sprint you can see how the contact matrices for AA, AB and BB are constructed separately and then concatentated into a single 
object.  You can also see how the process of sorting the components of the eigenvector has to be modified to take account of the fact 
that all the atoms are not indistinguishable.  In conclusion, my hope is that readers can make sense of the way CVs are constructed from
shortcut in PLUMED by reading the original paper and the PLUMED input files together.




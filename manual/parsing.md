Parsing action input 
-------------------- 

The input to any PLUMED [action](actions.md) consists of a series of keyword value pairs and flags that turn on or off various options. 
In the example input below: 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_parsing.md_working_1.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="parsing.md_working_1.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="parsing.md_working_1.datd1" onclick='showPath("parsing.md_working_1.dat","parsing.md_working_1.datd1","parsing.md_working_1.datd1","black")'>d1</b><span style="display:none;" id="parsing.md_working_1.datd1">The DISTANCE action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1</td><td width="5%"><font color="black">scalar</font></td><td>the DISTANCE between this pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=1,2 <div class="tooltip">NOPBC<div class="right"> ignore the periodic boundary conditions when calculating distances<i></i></div></div>
</pre>
 {% endraw %} 

`d1` is the action's [label](specifying_arguments.md) and `DISTANCE` is the action's name. The input to the action is then the keyword value pair ATOMS and the flag NOPBC. 
Every example input you encounter in this manual, in the [nest](www.plumed-nest.org) and the [tutorials](www.plumed-tutorials.org) has tooltips 
that explain what options are turned on by flags and what the values provided in each keyword pair represents. You will also find details of 
all the keywords and flags that are available for an action on the manual page for that action. 

## Reading constants 

In the input to keywords that read real numbers you can use constants that are specified using strings rather than numbers. 
An example is the following 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_parsing.md_working_2.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="parsing.md_working_2.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#SETTINGS MOLFILE=regtest/basic/rt65/AA.pdb</span>
<div class="tooltip" style="color:green">MOLINFO<div class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRUCTURE<div class="right">a file in pdb format containing a reference structure<i></i></div></div>=AA.pdb  <div class="tooltip">MOLTYPE<div class="right"> what kind of molecule is contained in the pdb file - usually not needed since protein/RNA/DNA are compatible<i></i></div></div>=rna
<span style="display:none;" id="parsing.md_working_2.dat">The MOLINFO action with label <b></b> calculates something</span><b name="parsing.md_working_2.date1" onclick='showPath("parsing.md_working_2.dat","parsing.md_working_2.date1","parsing.md_working_2.date1","brown")'>e1</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=<div class="tooltip">@epsilon-1<div class="right">the four atoms that are required to calculate the backbone epsilon dihedral for residue 1. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>
<span style="display:none;" id="parsing.md_working_2.date1">The TORSION action with label <b>e1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">e1.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="parsing.md_working_2.datt" onclick='showPath("parsing.md_working_2.dat","parsing.md_working_2.datt","parsing.md_working_2.datt","brown")'>t</b>: <div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalars on which the bias will act<i></i></div></div>=<b name="parsing.md_working_2.date1">e1</b> <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.15 <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=10 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=2 <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=-pi <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=pi <div class="tooltip">GRID_BIN<div class="right">the number of bins for the grid<i></i></div></div>=200
<span style="display:none;" id="parsing.md_working_2.datt">The METAD action with label <b>t</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">t.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span></pre>
 {% endraw %} 

Notice here that the boundaries for `GRID_MIN` and `GRID_MAX` are `-pi` and `pi`. 

Any real numbers that are read in from input are interpretted using the [Lepton library](Custom.md) so you can thus employ 
complicated expressions such as `1+2` or `exp(10)` as shown in the in the input as shown below: 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_parsing.md_working_3.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="parsing.md_working_3.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#SETTINGS MOLFILE=regtest/basic/rt65/AA.pdb</span>
<div class="tooltip" style="color:green">MOLINFO<div class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRUCTURE<div class="right">a file in pdb format containing a reference structure<i></i></div></div>=AA.pdb  <div class="tooltip">MOLTYPE<div class="right"> what kind of molecule is contained in the pdb file - usually not needed since protein/RNA/DNA are compatible<i></i></div></div>=rna
<span style="display:none;" id="parsing.md_working_3.dat">The MOLINFO action with label <b></b> calculates something</span><b name="parsing.md_working_3.date1" onclick='showPath("parsing.md_working_3.dat","parsing.md_working_3.date1","parsing.md_working_3.date1","brown")'>e1</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=<div class="tooltip">@epsilon-1<div class="right">the four atoms that are required to calculate the backbone epsilon dihedral for residue 1. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>
<span style="display:none;" id="parsing.md_working_3.date1">The TORSION action with label <b>e1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">e1.value</td><td>the TORSION involving these atoms</td></tr></table></span><div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="parsing.md_working_3.date1">e1</b> <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=1+0.5
</pre>
 {% endraw %} 

The lepton library is able to interpret any of thse following constants: 

| Symbol | Description | 
| :----- |:------------| 
| `e` | Euler's number - the base for the natural logarithm | 
| `log2e` | $1 / \log(2)$ | 
| `log10e` | $1 / \log(10)$ | 
| `ln2` | $\log(2)$ | 
| `ln10` | $\log(10)$ | 
| `pi` | the circle constant $\pi$ | 
| `pi_2` | $\pi / 2$ | 
| `pi_4` | $\pi / 4$ | 
| `sqrt2 | $\sqrt(2)$ | 
| `sqrt1_2 ` | $\sqrt(0.5)$ | 

Notice that this functionality cannot be used when the keyword takes integer numbers in input 
(e.g.: the PACE argument for METAD). 

## Special replica syntax 

PLUMED provides a number of ways to prepare the multiple replicas with almost identical PLUMED files that are required to run a multiple replica simulation: 

* You can repare input files for such calculation using cut-and-paste but that is is very error prone. 
* You can write a smart bash or python script to generate all the inputs. 
* You can use different inputs for the various replicas that all contain an [INCLUDE](INCLUDE.md) directive to include a file that contains the parts of the input that are common to all replicas 

We think, however, the best option is to use features that have been available from PLUMED 2.4 onwards that allow you 
manipulate multiple replica inputs that have only tiny differences in the the input. The following example illustrates how the syntax 
for this option operates: 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_parsing.md_working_4.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="parsing.md_working_4.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#SETTINGS NREPLICAS=3</span>
<span style="color:blue" class="comment"># Compute a distance</span>
<b name="parsing.md_working_4.datd" onclick='showPath("parsing.md_working_4.dat","parsing.md_working_4.datd","parsing.md_working_4.datd","brown")'>d</b>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=1,2
<br/><span style="color:blue" class="comment"># Apply a restraint.</span>
<span style="display:none;" id="parsing.md_working_4.datd">The DISTANCE action with label <b>d</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="parsing.md_working_4.datd">d</b> <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=<div class="tooltip">@replicas:<div class="right">This keyword specifies that different replicas have different values for this quantity.  See <a href="https://www.plumed.org/doc-master/user-doc/html/special-replica-syntax.html">here for more details.</a><i></i></div></div>1.0,1.1,1.2 <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=1.0
<span style="color:blue" class="comment"># On replica 0, this means:</span>
<span style="color:blue" class="comment">#   RESTRAINT ARG=d AT=1.0 KAPPA=1.0</span>
<span style="color:blue" class="comment"># On replica 1, this means:</span>
<span style="color:blue" class="comment">#   RESTRAINT ARG=d AT=1.1 KAPPA=1.0</span>
<span style="color:blue" class="comment"># On replica 2, this means:</span>
<span style="color:blue" class="comment">#   RESTRAINT ARG=d AT=1.2 KAPPA=1.0</span>
</pre>
 {% endraw %} 

If you prepare a single `plumed.dat` file like this one and feeds it to PLUMED while using 3 replicas, 
the 3 replicas will see PLUMED input files that are the same except for the `AT` keyword, that sets the position of the restraint. 
Replica 0 will see a restraint centered at 1.0, replica 1 centered at 1.1, and replica 2 centered at 1.2. 

The `@replicas:` keyword is not specific to RESTRAINT and the `AT` keyword. Any keyword in PLUMED can accept that syntax. 
For instance, the following single input file can be used to [setup](setup.md) a [bias](bias.md) exchange metadynamics simulations: 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_parsing.md_working_5.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="parsing.md_working_5.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#SETTINGS NREPLICAS=2 </span>
<span style="color:blue" class="comment"># Compute distance between atoms 1 and 2</span>
<b name="parsing.md_working_5.datd" onclick='showPath("parsing.md_working_5.dat","parsing.md_working_5.datd","parsing.md_working_5.datd","black")'>d</b><span style="display:none;" id="parsing.md_working_5.datd">The DISTANCE action with label <b>d</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d</td><td width="5%"><font color="black">scalar</font></td><td>the DISTANCE between this pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=1,2
<br/><span style="color:blue" class="comment"># Compute a torsional angle </span>
<b name="parsing.md_working_5.datt" onclick='showPath("parsing.md_working_5.dat","parsing.md_working_5.datt","parsing.md_working_5.datt","black")'>t</b><span style="display:none;" id="parsing.md_working_5.datt">The TORSION action with label <b>t</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">t</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=30,31,32,33
<br/><span style="color:blue" class="comment"># Metadynamics.</span>
<div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the labels of the scalars on which the bias will act<i></i></div></div>=<div class="tooltip">@replicas:<div class="right">This keyword specifies that different replicas have different values for this quantity.  See <a href="https://www.plumed.org/doc-master/user-doc/html/special-replica-syntax.html">here for more details.</a><i></i></div></div><b name="parsing.md_working_5.datd">d</b>,<b name="parsing.md_working_5.datt">t</b>
  <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=1.0
  <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=100
  <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=<div class="tooltip">@replicas:<div class="right">This keyword specifies that different replicas have different values for this quantity.  See <a href="https://www.plumed.org/doc-master/user-doc/html/special-replica-syntax.html">here for more details.</a><i></i></div></div>0.1,0.3
  <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=<div class="tooltip">@replicas:<div class="right">This keyword specifies that different replicas have different values for this quantity.  See <a href="https://www.plumed.org/doc-master/user-doc/html/special-replica-syntax.html">here for more details.</a><i></i></div></div>0.0,-pi
  <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=<div class="tooltip">@replicas:<div class="right">This keyword specifies that different replicas have different values for this quantity.  See <a href="https://www.plumed.org/doc-master/user-doc/html/special-replica-syntax.html">here for more details.</a><i></i></div></div>2.0,pi
...
<span style="color:blue" class="comment"># On replica 0, this means:</span>
<span style="color:blue" class="comment">#  METAD ARG=d HEIGHT=1.0 PACE=100 SIGMA=0.1 GRID_MIN=0.0 GRID_MAX=2.0</span>
<span style="color:blue" class="comment"># On replica 1, this means:</span>
<span style="color:blue" class="comment">#  METAD ARG=t HEIGHT=1.0 PACE=100 SIGMA=0.3 GRID_MIN=-pi GRID_MAX=pi</span>
</pre>
 {% endraw %} 

This input contains a typical [setup](setup.md) for a [bias](bias.md) exchange simulation. 
Notice that even though the actions with labels `d` and `t` are read for both replicas, 
`d` is only computed on replica 0 (and `t` is only computed on replica 1). 
This is because variables that are defined but not used are never actually calculated by PLUMED. 

If the value that should be provided for each replica is a vector, you should use curly braces as delimiters. 
For instance, if you have a restraint that acts on two variables, you can use the following input: 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_parsing.md_working_6.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="parsing.md_working_6.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#SETTINGS NREPLICAS=3</span>
<span style="color:blue" class="comment"># Compute distance between atoms 1 and 2</span>
<b name="parsing.md_working_6.datd" onclick='showPath("parsing.md_working_6.dat","parsing.md_working_6.datd","parsing.md_working_6.datd","brown")'>d</b>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=10,20
<br/><span style="color:blue" class="comment"># Compute a torsional angle</span>
<span style="display:none;" id="parsing.md_working_6.datd">The DISTANCE action with label <b>d</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><b name="parsing.md_working_6.datt" onclick='showPath("parsing.md_working_6.dat","parsing.md_working_6.datt","parsing.md_working_6.datt","brown")'>t</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=30,31,32,33
<br/><span style="color:blue" class="comment"># Apply a restraint:</span>
<span style="display:none;" id="parsing.md_working_6.datt">The TORSION action with label <b>t</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">t.value</td><td>the TORSION involving these atoms</td></tr></table></span><div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="parsing.md_working_6.datd">d</b>,<b name="parsing.md_working_6.datt">t</b>
  <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=<div class="tooltip">@replicas:<div class="right">This keyword specifies that different replicas have different values for this quantity.  See <a href="https://www.plumed.org/doc-master/user-doc/html/special-replica-syntax.html">here for more details.</a><i></i></div></div>{{1.0,2.0} 3040 5060
  <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=1.0,3.0
...
<span style="color:blue" class="comment"># On replica 0 this means:</span>
<span style="color:blue" class="comment">#  RESTRAINT ARG=d AT=1.0,2.0 KAPPA=1.0,3.0</span>
<span style="color:blue" class="comment"># On replica 1 this means:</span>
<span style="color:blue" class="comment">#  RESTRAINT ARG=d AT=3.0,4.0 KAPPA=1.0,3.0</span>
<span style="color:blue" class="comment"># On replica 2 this means:</span>
<span style="color:blue" class="comment">#  RESTRAINT ARG=d AT=5.0,6.0 KAPPA=1.0,3.0</span>
</pre>
 {% endraw %} 

Notice the double curly braces. The outer ones are used by PLUMED to know where the argument of the `AT` keyword ends, 
whereas the inner ones are used to group the values corresponding to each replica. 
Also notice that the last example can be split in multiple lines exploiting the fact that 
within multi-line statements (enclosed by pairs of `...`) newlines are replaced with simple spaces: 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_parsing.md_working_7.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="parsing.md_working_7.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#SETTINGS NREPLICAS=3</span>
<b name="parsing.md_working_7.datd" onclick='showPath("parsing.md_working_7.dat","parsing.md_working_7.datd","parsing.md_working_7.datd","brown")'>d</b>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=10,20
<span style="display:none;" id="parsing.md_working_7.datd">The DISTANCE action with label <b>d</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><b name="parsing.md_working_7.datt" onclick='showPath("parsing.md_working_7.dat","parsing.md_working_7.datt","parsing.md_working_7.datt","brown")'>t</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=30,31,32,33
<span style="display:none;" id="parsing.md_working_7.datt">The TORSION action with label <b>t</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">t.value</td><td>the TORSION involving these atoms</td></tr></table></span><div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="parsing.md_working_7.datd">d</b>,<b name="parsing.md_working_7.datt">t</b>
<span style="color:blue" class="comment"># indentation is not required (this is not python!)</span>
<span style="color:blue" class="comment"># but makes the input easier to read</span>
  <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=<div class="tooltip">@replicas:<div class="right">This keyword specifies that different replicas have different values for this quantity.  See <a href="https://www.plumed.org/doc-master/user-doc/html/special-replica-syntax.html">here for more details.</a><i></i></div></div>{
    {1.0,2.0}
    3040
    5060
  
  <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=1.0,3.0
...
</pre>
 {% endraw %} 

In short, whenever there are keywords that should vary across replicas, you should set them using the `@replicas:` keyword. 
As mentioned above, you can always use the old syntax with separate input files and this is fact recommended when the 
differences in the inputs for the various replicas are substantial. 


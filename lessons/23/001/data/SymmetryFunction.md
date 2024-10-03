# Calculating symmetry functions

In the other blog articles on these pages I have written a great deal about how you can calculate coordination numbers 
using inputs such as the one below:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_SymmetryFunction.md_working_1.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="SymmetryFunction.md_working_1.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="SymmetryFunction.md_working_1.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Calculate the contact matrix.  This is a square 7x7 matrix</span>
<b name="SymmetryFunction.md_working_1.datc1" onclick='showPath("SymmetryFunction.md_working_1.dat","SymmetryFunction.md_working_1.datc1","SymmetryFunction.md_working_1.datc1","red")'>c1</b><span style="display:none;" id="SymmetryFunction.md_working_1.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=1-7 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=2.6 NN=6 MM=12}
<span style="color:blue" class="comment"># Calculate the coordination numbers for the 7 atoms by a vector that contains all ones</span>
<span id="SymmetryFunction.md_working_1.datones_short"><b name="SymmetryFunction.md_working_1.datones" onclick='showPath("SymmetryFunction.md_working_1.dat","SymmetryFunction.md_working_1.datones","SymmetryFunction.md_working_1.datones_shortcut","blue")'>ones</b><span style="display:none;" id="SymmetryFunction.md_working_1.datones_shortcut">The ONES action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("SymmetryFunction.md_working_1.datones");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=7
</span><span id="SymmetryFunction.md_working_1.datones_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("SymmetryFunction.md_working_1.datones")'># ones: ONES SIZE=7</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="SymmetryFunction.md_working_1.datones" onclick='showPath("SymmetryFunction.md_working_1.dat","SymmetryFunction.md_working_1.datones","SymmetryFunction.md_working_1.datones","blue")'>ones</b><span style="display:none;" id="SymmetryFunction.md_working_1.datones">The CONSTANT action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><b name="SymmetryFunction.md_working_1.datcc" onclick='showPath("SymmetryFunction.md_working_1.dat","SymmetryFunction.md_working_1.datcc","SymmetryFunction.md_working_1.datcc","blue")'>cc</b><span style="display:none;" id="SymmetryFunction.md_working_1.datcc">The MATRIX_VECTOR_PRODUCT action with label <b>cc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="SymmetryFunction.md_working_1.datc1">c1</b>,<b name="SymmetryFunction.md_working_1.datones">ones</b>
<span style="color:blue" class="comment"># And output the 7 coordination numbers for the atoms</span>
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the values that you would like to print to the file<i></i></div></div>=<b name="SymmetryFunction.md_working_1.datcc">cc</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

In this article I want to explain how we can use PLUMED input files that are similar to the one above to calculate 
other input files.

## CONTACT_MATRIX and the COMPONENTS flag

In the input at the top of this file I used a CONTACT_MATRIX.  This command outputs a matrix, $\mathbf{A}$, in which element $i,j$ is given by:

$$
A_{ij} = \sigma(r_{ij})
$$

where $\sigma$ is a switching function and $r_{ij}$ is the distance between atom $i$ and atom $j$.  

Switching functions like $\sigma(r_{ij})$ are used in the definitions symmetry functions such as those used in the FCCUBIC, TETRAHEDRAL and SIMPLECUBIC actions.  These functions have the following general form:

$$
s_i = \sum_{j\ne i } f(x_{ij},y_{ij},z_{ij})\sigma(r_{ij})
$$

where $f$ is some function of the $x_{ij}$, $y_{ij}$ and $z_{ij}$ components of the vector that connects atom $i$ to atom $j$.  To make it easy to implement such functions I have introduced a 
COMPONENTS flag on the CONTACT_MATRIX command that can be used as shown below:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_SymmetryFunction.md_working_2.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="SymmetryFunction.md_working_2.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="SymmetryFunction.md_working_2.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Calculate the contact matrix and the three matrices that contain the components of the vectors connecting atom i and atom j.  In other words, calculate four 7x7 matrices</span>
<b name="SymmetryFunction.md_working_2.datc1" onclick='showPath("SymmetryFunction.md_working_2.dat","SymmetryFunction.md_working_2.datc1","SymmetryFunction.md_working_2.datc1","red")'>c1</b><span style="display:none;" id="SymmetryFunction.md_working_2.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1.w</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr><tr><td width="5%">c1.x</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the x axis</td></tr><tr><td width="5%">c1.y</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the y axis</td></tr><tr><td width="5%">c1.z</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the z axis</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">COMPONENTS<div class="right"> also calculate the components of the vector connecting the atoms in the contact matrix<i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=1-7 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=2.6 NN=6 MM=12}
<span style="color:blue" class="comment"># Output the four 7x7 matrices calculated by the command above to a file.</span>
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the values that you would like to print to the file<i></i></div></div>=<b name="SymmetryFunction.md_working_2.datc1">c1.w</b>,<b name="SymmetryFunction.md_working_2.datc1">c1.x</b>,<b name="SymmetryFunction.md_working_2.datc1">c1.y</b>,<b name="SymmetryFunction.md_working_2.datc1">c1.z</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

The COMPONENTS flag for the CONTACT_MATRIX action is specfically designed to make calculating symmetry functions such as $s_i$ striaghforward.  The elements of the matrix `c1.x` are 
thus calculated as:

$$
X_{ij} = \begin{cases}
x_{ij} & \textrm{if} \quad \sigma(r_{ij})>0 \\
0 & \textrm{otherwise}
\end{cases}
$$

The elements of `c1.y` and `c1.z` are also calculated in a similar fashion.  __In other words, the $i,j$ element of these three matrices are only non-zero if atom $j$ is within the first coordination sphere 
of atom $i$.__

## Combining CONTACT_MATRIX and CUSTOM

We can use the CONTACT_MATRIX command with the COMPONENTS keyword to calculate a function similar to $s_i$ above as follows:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_SymmetryFunction.md_working_3.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="SymmetryFunction.md_working_3.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="SymmetryFunction.md_working_3.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Calculate the contact matrix and the three matrices that contain the components of the vectors connecting atom i and atom j.  In other words, calculate four 7x7 matrices</span>
<b name="SymmetryFunction.md_working_3.datc1" onclick='showPath("SymmetryFunction.md_working_3.dat","SymmetryFunction.md_working_3.datc1","SymmetryFunction.md_working_3.datc1","red")'>c1</b><span style="display:none;" id="SymmetryFunction.md_working_3.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1.w</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr><tr><td width="5%">c1.x</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the x axis</td></tr><tr><td width="5%">c1.y</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the y axis</td></tr><tr><td width="5%">c1.z</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the z axis</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">COMPONENTS<div class="right"> also calculate the components of the vector connecting the atoms in the contact matrix<i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=1-7 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=2.6 NN=6 MM=12}
<span style="color:blue" class="comment"># This applies the function to the three input matrices element-wise and thus outputs a 7x7 matrix</span>
<b name="SymmetryFunction.md_working_3.datr" onclick='showPath("SymmetryFunction.md_working_3.dat","SymmetryFunction.md_working_3.datr","SymmetryFunction.md_working_3.datr","red")'>r</b><span style="display:none;" id="SymmetryFunction.md_working_3.datr">The CUSTOM action with label <b>r</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">r</td><td width="5%"><font color="red">matrix</font></td><td>the matrix obtained by doing an element-wise application of an arbitrary function to the input matrix</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="SymmetryFunction.md_working_3.datc1">c1.x</b>,<b name="SymmetryFunction.md_working_3.datc1">c1.y</b>,<b name="SymmetryFunction.md_working_3.datc1">c1.z</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=sqrt(x*x+y*y+z*z <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<span style="color:blue" class="comment"># Again we are applying the function element wise to the five input matrices and thus outputting a 7x7 matrix</span>
<b name="SymmetryFunction.md_working_3.datf" onclick='showPath("SymmetryFunction.md_working_3.dat","SymmetryFunction.md_working_3.datf","SymmetryFunction.md_working_3.datf","red")'>f</b><span style="display:none;" id="SymmetryFunction.md_working_3.datf">The CUSTOM action with label <b>f</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">f</td><td width="5%"><font color="red">matrix</font></td><td>the matrix obtained by doing an element-wise application of an arbitrary function to the input matrix</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="SymmetryFunction.md_working_3.datc1">c1.w</b>,<b name="SymmetryFunction.md_working_3.datc1">c1.x</b>,<b name="SymmetryFunction.md_working_3.datc1">c1.y</b>,<b name="SymmetryFunction.md_working_3.datc1">c1.z</b>,<b name="SymmetryFunction.md_working_3.datr">r</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=w*(x^4+y^4+z^4)/(r^4 <div class="tooltip">VAR<div class="right">the names to give each of the arguments in the function<i></i></div></div>=w,x,y,z,<b name="SymmetryFunction.md_working_3.datr">r</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<span style="color:blue" class="comment"># We now multiply the 7x7 by a vector of ones to calculate the symmetry function</span>
<span id="SymmetryFunction.md_working_3.datones_short"><b name="SymmetryFunction.md_working_3.datones" onclick='showPath("SymmetryFunction.md_working_3.dat","SymmetryFunction.md_working_3.datones","SymmetryFunction.md_working_3.datones_shortcut","blue")'>ones</b><span style="display:none;" id="SymmetryFunction.md_working_3.datones_shortcut">The ONES action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("SymmetryFunction.md_working_3.datones");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=7
</span><span id="SymmetryFunction.md_working_3.datones_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("SymmetryFunction.md_working_3.datones")'># ones: ONES SIZE=7</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="SymmetryFunction.md_working_3.datones" onclick='showPath("SymmetryFunction.md_working_3.dat","SymmetryFunction.md_working_3.datones","SymmetryFunction.md_working_3.datones","blue")'>ones</b><span style="display:none;" id="SymmetryFunction.md_working_3.datones">The CONSTANT action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><b name="SymmetryFunction.md_working_3.dats" onclick='showPath("SymmetryFunction.md_working_3.dat","SymmetryFunction.md_working_3.dats","SymmetryFunction.md_working_3.dats","blue")'>s</b><span style="display:none;" id="SymmetryFunction.md_working_3.dats">The MATRIX_VECTOR_PRODUCT action with label <b>s</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">s</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="SymmetryFunction.md_working_3.datf">f</b>,<b name="SymmetryFunction.md_working_3.datones">ones</b> 
<span style="color:blue" class="comment"># And print the sum of the symmetry function to a file</span>
<b name="SymmetryFunction.md_working_3.datsums" onclick='showPath("SymmetryFunction.md_working_3.dat","SymmetryFunction.md_working_3.datsums","SymmetryFunction.md_working_3.datsums","black")'>sums</b><span style="display:none;" id="SymmetryFunction.md_working_3.datsums">The SUM action with label <b>sums</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">sums</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="SymmetryFunction.md_working_3.dats">s</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the values that you would like to print to the file<i></i></div></div>=<b name="SymmetryFunction.md_working_3.datsums">sums</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

The graph for this input is shown below:

```mermaid
flowchart TB 
MD(positions from MD)
Box("label=Box 
 PBC 
")
Box -- Box --> c1
linkStyle 0 stroke:red,color:red;
MD --> c1
linkStyle 1 stroke:violet,color:violet;
subgraph subc1 [c1]
subgraph subc1_mat [c1]
c1(["label=c1 
 CONTACT_MATRIX 
"])
r(["label=r 
 CUSTOM
FUNC=sqrt(x*x+y*y+z*z) 
"])
f(["label=f 
 CUSTOM
FUNC=w*(x^4+y^4+z^4)/(r^4) 
"])
s(["label=s 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subc1_mat fill:lightblue
sums(["label=sums 
 SUM 
"])
end
c1 -- c1.x --> r
linkStyle 2 stroke:red,color:red;
c1 -- c1.y --> r
linkStyle 3 stroke:red,color:red;
c1 -- c1.z --> r
linkStyle 4 stroke:red,color:red;
c1 -- c1.w --> f
linkStyle 5 stroke:red,color:red;
c1 -- c1.x --> f
linkStyle 6 stroke:red,color:red;
c1 -- c1.y --> f
linkStyle 7 stroke:red,color:red;
c1 -- c1.z --> f
linkStyle 8 stroke:red,color:red;
r -- r --> f
linkStyle 9 stroke:red,color:red;
ones(["label=ones 
 CONSTANT 
"])
f -- f --> s
linkStyle 10 stroke:red,color:red;
ones -- ones --> s
linkStyle 11 stroke:blue,color:blue;
s -- s --> sums
linkStyle 12 stroke:blue,color:blue;
sums -- sums --> 11
11("label=#64;11 
 PRINT
FILE=colvar 
")

```
{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_SymmetryFunction.md_working_4.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="SymmetryFunction.md_working_4.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="SymmetryFunction.md_working_4.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Calculate the contact matrix and the three matrices that contain the components of the vectors connecting atom i and atom j.  In other words, calculate four 7x7 matrices</span>
<b name="SymmetryFunction.md_working_4.datc1" onclick='showPath("SymmetryFunction.md_working_4.dat","SymmetryFunction.md_working_4.datc1","SymmetryFunction.md_working_4.datc1","red")'>c1</b><span style="display:none;" id="SymmetryFunction.md_working_4.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1.w</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr><tr><td width="5%">c1.x</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the x axis</td></tr><tr><td width="5%">c1.y</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the y axis</td></tr><tr><td width="5%">c1.z</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the z axis</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">COMPONENTS<div class="right"> also calculate the components of the vector connecting the atoms in the contact matrix<i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=1-7 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=2.6 NN=6 MM=12}
<span style="color:blue" class="comment"># This applies the function to the three input matrices element-wise and thus outputs a 7x7 matrix</span>
<b name="SymmetryFunction.md_working_4.datr" onclick='showPath("SymmetryFunction.md_working_4.dat","SymmetryFunction.md_working_4.datr","SymmetryFunction.md_working_4.datr","red")'>r</b><span style="display:none;" id="SymmetryFunction.md_working_4.datr">The CUSTOM action with label <b>r</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">r</td><td width="5%"><font color="red">matrix</font></td><td>the matrix obtained by doing an element-wise application of an arbitrary function to the input matrix</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="SymmetryFunction.md_working_4.datc1">c1.x</b>,<b name="SymmetryFunction.md_working_4.datc1">c1.y</b>,<b name="SymmetryFunction.md_working_4.datc1">c1.z</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=sqrt(x*x+y*y+z*z <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<span style="color:blue" class="comment"># Again we are applying the function element wise to the five input matrices and thus outputting a 7x7 matrix</span>
<b name="SymmetryFunction.md_working_4.datf" onclick='showPath("SymmetryFunction.md_working_4.dat","SymmetryFunction.md_working_4.datf","SymmetryFunction.md_working_4.datf","red")'>f</b><span style="display:none;" id="SymmetryFunction.md_working_4.datf">The CUSTOM action with label <b>f</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">f</td><td width="5%"><font color="red">matrix</font></td><td>the matrix obtained by doing an element-wise application of an arbitrary function to the input matrix</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="SymmetryFunction.md_working_4.datc1">c1.w</b>,<b name="SymmetryFunction.md_working_4.datc1">c1.x</b>,<b name="SymmetryFunction.md_working_4.datc1">c1.y</b>,<b name="SymmetryFunction.md_working_4.datc1">c1.z</b>,<b name="SymmetryFunction.md_working_4.datr">r</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=w*(x^4+y^4+z^4)/(r^4 <div class="tooltip">VAR<div class="right">the names to give each of the arguments in the function<i></i></div></div>=w,x,y,z,<b name="SymmetryFunction.md_working_4.datr">r</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<span style="color:blue" class="comment"># We now multiply the 7x7 by a vector of ones to calculate the symmetry function</span>
<span id="SymmetryFunction.md_working_4.datones_short"><b name="SymmetryFunction.md_working_4.datones" onclick='showPath("SymmetryFunction.md_working_4.dat","SymmetryFunction.md_working_4.datones","SymmetryFunction.md_working_4.datones_shortcut","blue")'>ones</b><span style="display:none;" id="SymmetryFunction.md_working_4.datones_shortcut">The ONES action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("SymmetryFunction.md_working_4.datones");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=7
</span><span id="SymmetryFunction.md_working_4.datones_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("SymmetryFunction.md_working_4.datones")'># ones: ONES SIZE=7</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="SymmetryFunction.md_working_4.datones" onclick='showPath("SymmetryFunction.md_working_4.dat","SymmetryFunction.md_working_4.datones","SymmetryFunction.md_working_4.datones","blue")'>ones</b><span style="display:none;" id="SymmetryFunction.md_working_4.datones">The CONSTANT action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><b name="SymmetryFunction.md_working_4.dats" onclick='showPath("SymmetryFunction.md_working_4.dat","SymmetryFunction.md_working_4.dats","SymmetryFunction.md_working_4.dats","blue")'>s</b><span style="display:none;" id="SymmetryFunction.md_working_4.dats">The MATRIX_VECTOR_PRODUCT action with label <b>s</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">s</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="SymmetryFunction.md_working_4.datf">f</b>,<b name="SymmetryFunction.md_working_4.datones">ones</b>
<span style="color:blue" class="comment"># And print the sum of the symmetry function to a file</span>
<b name="SymmetryFunction.md_working_4.datsums" onclick='showPath("SymmetryFunction.md_working_4.dat","SymmetryFunction.md_working_4.datsums","SymmetryFunction.md_working_4.datsums","black")'>sums</b><span style="display:none;" id="SymmetryFunction.md_working_4.datsums">The SUM action with label <b>sums</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">sums</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="SymmetryFunction.md_working_4.dats">s</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the values that you would like to print to the file<i></i></div></div>=<b name="SymmetryFunction.md_working_4.datsums">sums</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

Notice that all the commands are done in a single chain.  There is no need to store any matrix elements as the functions in `r` and `f` are applied to the elements of the matrices calculated
by `c1` immediately after they are calculated.  Furthermore, if one were to sum the elements of the vector `s` and add a bias upon the sum, the forces on `s` are passed back through the code as
shown below:

```mermaid
flowchart TB 
MD(positions from MD)
Box("label=Box 
 PBC 
")
Box -- Box --> c1
linkStyle 0 stroke:red,color:red;
MD --> c1
linkStyle 1 stroke:violet,color:violet;
subgraph subc1 [c1]
subgraph subc1_mat [c1]
c1(["label=c1 
 CONTACT_MATRIX 
"])
r(["label=r 
 CUSTOM
FUNC=sqrt(x*x+y*y+z*z) 
"])
f(["label=f 
 CUSTOM
FUNC=w*(x^4+y^4+z^4)/(r^4) 
"])
s(["label=s 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subc1_mat fill:lightblue
sums(["label=sums 
 SUM 
"])
end
c1 -- c1.x --> r
linkStyle 2 stroke:red,color:red;
c1 -- c1.y --> r
linkStyle 3 stroke:red,color:red;
c1 -- c1.z --> r
linkStyle 4 stroke:red,color:red;
c1 -- c1.w --> f
linkStyle 5 stroke:red,color:red;
c1 -- c1.x --> f
linkStyle 6 stroke:red,color:red;
c1 -- c1.y --> f
linkStyle 7 stroke:red,color:red;
c1 -- c1.z --> f
linkStyle 8 stroke:red,color:red;
r -- r --> f
linkStyle 9 stroke:red,color:red;
ones(["label=ones 
 CONSTANT 
"])
f -- f --> s
linkStyle 10 stroke:red,color:red;
ones -- ones --> s
linkStyle 11 stroke:blue,color:blue;
s -- s --> sums
linkStyle 12 stroke:blue,color:blue;
sums -- sums --> 11
11("label=#64;11 
 PRINT
FILE=colvar 
")

```
{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_SymmetryFunction.md_working_5.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="SymmetryFunction.md_working_5.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="SymmetryFunction.md_working_5.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Calculate the contact matrix and the three matrices that contain the components of the vectors connecting atom i and atom j.  In other words, calculate four 7x7 matrices</span>
<b name="SymmetryFunction.md_working_5.datc1" onclick='showPath("SymmetryFunction.md_working_5.dat","SymmetryFunction.md_working_5.datc1","SymmetryFunction.md_working_5.datc1","red")'>c1</b><span style="display:none;" id="SymmetryFunction.md_working_5.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1.w</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr><tr><td width="5%">c1.x</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the x axis</td></tr><tr><td width="5%">c1.y</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the y axis</td></tr><tr><td width="5%">c1.z</td><td width="5%"><font color="red">matrix</font></td><td>the projection of the bond on the z axis</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">COMPONENTS<div class="right"> also calculate the components of the vector connecting the atoms in the contact matrix<i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=1-7 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=2.6 NN=6 MM=12}
<span style="color:blue" class="comment"># This applies the function to the three input matrices element-wise and thus outputs a 7x7 matrix</span>
<b name="SymmetryFunction.md_working_5.datr" onclick='showPath("SymmetryFunction.md_working_5.dat","SymmetryFunction.md_working_5.datr","SymmetryFunction.md_working_5.datr","red")'>r</b><span style="display:none;" id="SymmetryFunction.md_working_5.datr">The CUSTOM action with label <b>r</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">r</td><td width="5%"><font color="red">matrix</font></td><td>the matrix obtained by doing an element-wise application of an arbitrary function to the input matrix</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="SymmetryFunction.md_working_5.datc1">c1.x</b>,<b name="SymmetryFunction.md_working_5.datc1">c1.y</b>,<b name="SymmetryFunction.md_working_5.datc1">c1.z</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=sqrt(x*x+y*y+z*z <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<span style="color:blue" class="comment"># Again we are applying the function element wise to the five input matrices and thus outputting a 7x7 matrix</span>
<b name="SymmetryFunction.md_working_5.datf" onclick='showPath("SymmetryFunction.md_working_5.dat","SymmetryFunction.md_working_5.datf","SymmetryFunction.md_working_5.datf","red")'>f</b><span style="display:none;" id="SymmetryFunction.md_working_5.datf">The CUSTOM action with label <b>f</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">f</td><td width="5%"><font color="red">matrix</font></td><td>the matrix obtained by doing an element-wise application of an arbitrary function to the input matrix</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="SymmetryFunction.md_working_5.datc1">c1.w</b>,<b name="SymmetryFunction.md_working_5.datc1">c1.x</b>,<b name="SymmetryFunction.md_working_5.datc1">c1.y</b>,<b name="SymmetryFunction.md_working_5.datc1">c1.z</b>,<b name="SymmetryFunction.md_working_5.datr">r</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=w*(x^4+y^4+z^4)/(r^4 <div class="tooltip">VAR<div class="right">the names to give each of the arguments in the function<i></i></div></div>=w,x,y,z,<b name="SymmetryFunction.md_working_5.datr">r</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<span style="color:blue" class="comment"># We now multiply the 7x7 by a vector of ones to calculate the symmetry function</span>
<span id="SymmetryFunction.md_working_5.datones_short"><b name="SymmetryFunction.md_working_5.datones" onclick='showPath("SymmetryFunction.md_working_5.dat","SymmetryFunction.md_working_5.datones","SymmetryFunction.md_working_5.datones_shortcut","blue")'>ones</b><span style="display:none;" id="SymmetryFunction.md_working_5.datones_shortcut">The ONES action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("SymmetryFunction.md_working_5.datones");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=7
</span><span id="SymmetryFunction.md_working_5.datones_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("SymmetryFunction.md_working_5.datones")'># ones: ONES SIZE=7</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="SymmetryFunction.md_working_5.datones" onclick='showPath("SymmetryFunction.md_working_5.dat","SymmetryFunction.md_working_5.datones","SymmetryFunction.md_working_5.datones","blue")'>ones</b><span style="display:none;" id="SymmetryFunction.md_working_5.datones">The CONSTANT action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><b name="SymmetryFunction.md_working_5.dats" onclick='showPath("SymmetryFunction.md_working_5.dat","SymmetryFunction.md_working_5.dats","SymmetryFunction.md_working_5.dats","blue")'>s</b><span style="display:none;" id="SymmetryFunction.md_working_5.dats">The MATRIX_VECTOR_PRODUCT action with label <b>s</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">s</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="SymmetryFunction.md_working_5.datf">f</b>,<b name="SymmetryFunction.md_working_5.datones">ones</b>
<span style="color:blue" class="comment"># And print the sum of the symmetry function to a file</span>
<b name="SymmetryFunction.md_working_5.datsums" onclick='showPath("SymmetryFunction.md_working_5.dat","SymmetryFunction.md_working_5.datsums","SymmetryFunction.md_working_5.datsums","black")'>sums</b><span style="display:none;" id="SymmetryFunction.md_working_5.datsums">The SUM action with label <b>sums</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">sums</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="SymmetryFunction.md_working_5.dats">s</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the values that you would like to print to the file<i></i></div></div>=<b name="SymmetryFunction.md_working_5.datsums">sums</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

This is possible because the chain of actions the $(i,j)$ matrix elements for `r` and `f` (and their derivatives with respect to the atomic positions) are calculated immediately after $(i,j)$ matrix elements
for `c1.w`, `c1.x`, `c1.y` and `c1.z`.  In other words, in calculating `sums` we do a single loop over $i$ and $j$ and can thus accumulate values and derivatives without storing any matrices or vectors.

## Extending these symmetry functions

There are ways of defining the neighbourhood of atom $i$ that do not involve using the CONTACT_MATRIX keyword.  For example, you can define a matrix in which element $i,j$ is only non-zero if there is a hydrogen
bond between atom $i$ and atom $j$ (HBOND_MATRIX or HBPAMM_MATRIX) or, if you have molecules, you can say that molecule $i$ and $j$ are connected if they are within a cutoff of each other and if the two molecules
have some favourable orientation with respect to each other.  In all these cases you can also use a COMPONENTS keywords to get the direction of the bonds in the first coordination sphere as I have described in the 
article above.  You are thus not forced to use a switching function to define the $\sigma(r_{ij})$ part of the symmetry function that was defined above.  You can use other methods to determine whether atom $i$ and 
atom $j$ are adjacent or not.  Consequently, the implementation of these symmetry function in PLUMED is quite flexible and allows users to try many things without modifying the code.

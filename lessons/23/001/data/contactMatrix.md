# Contact matices and coordination numbers

The $i$, $j$ element of the conntact matrix, $\mathbf{C}_{ij}$, is one if atoms $i$ and $j$ are within a certain distance $r_c$ of each other and zero otherwise.
Consequently, if $\mathbf{C}$ is multiplied from the back by a vector of ones the $i$th element of the resulting matrix tells you the number of atoms that are 
within $r_c$ of atom $i$.  In other words, the coordination numbers of the atoms can be calculated from the contact matrix by doing matrix vector multiplication.

This realisation about the relationship between the contact map and the coordination number is heavily used in the new version of PLUMED.  For example, to calculate 
and print the coordination numbers of the first 7 atoms in the system with themselves you would use an input something like this:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_contactMatrix.md_working_1.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="contactMatrix.md_working_1.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="contactMatrix.md_working_1.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="contactMatrix.md_working_1.datc1" onclick='showPath("contactMatrix.md_working_1.dat","contactMatrix.md_working_1.datc1","contactMatrix.md_working_1.datc1","red")'>c1</b><span style="display:none;" id="contactMatrix.md_working_1.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=1-7 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=2.6 NN=6 MM=12}
<span id="contactMatrix.md_working_1.datones_short"><b name="contactMatrix.md_working_1.datones" onclick='showPath("contactMatrix.md_working_1.dat","contactMatrix.md_working_1.datones","contactMatrix.md_working_1.datones_shortcut","blue")'>ones</b><span style="display:none;" id="contactMatrix.md_working_1.datones_shortcut">The ONES action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_1.datones");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=7
</span><span id="contactMatrix.md_working_1.datones_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("contactMatrix.md_working_1.datones")'># ones: ONES SIZE=7</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="contactMatrix.md_working_1.datones" onclick='showPath("contactMatrix.md_working_1.dat","contactMatrix.md_working_1.datones","contactMatrix.md_working_1.datones","blue")'>ones</b><span style="display:none;" id="contactMatrix.md_working_1.datones">The CONSTANT action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><b name="contactMatrix.md_working_1.datcc" onclick='showPath("contactMatrix.md_working_1.dat","contactMatrix.md_working_1.datcc","contactMatrix.md_working_1.datcc","blue")'>cc</b><span style="display:none;" id="contactMatrix.md_working_1.datcc">The MATRIX_VECTOR_PRODUCT action with label <b>cc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_1.datc1">c1</b>,<b name="contactMatrix.md_working_1.datones">ones</b>
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the values that you would like to print to the file<i></i></div></div>=<b name="contactMatrix.md_working_1.datcc">cc</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

Implmenting the coordination number this way is useful as there are many different ways to define whether two atoms/molecules and to construct a "contact" matrix based on 
the result.  For example:

* You could say that two molecules are connected if they are within a certain distance of each other and if they have the same orientation.
* You could say that two water molecules are connected if they are hydrogen bonded to each other.
* You could say that two atoms are connected if they are within a certain distance of each other and if they have similar values for a CV.

When the coordination numbers is implemented in the way described above (by doing the matrix-vector multiplication) you have the flexibility to define the contact matrix that 
is used in the multiplication in whatever way you choose.  In other words, the newer implementation of the coordination number is much more flexible.

## Contact map chains

As discussed on [this page](MultiColvar.md), PLUMED avoids storing the derivatives for each element of a vector by creating a chain of actions instead of passing the vectors.  
We also use these chains of actions when passing matrices.  When we compute the CV defined by the input below:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_contactMatrix.md_working_2.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="contactMatrix.md_working_2.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="contactMatrix.md_working_2.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Calculate the contact matrix for the first seven atoms in the system</span>
<b name="contactMatrix.md_working_2.datc1" onclick='showPath("contactMatrix.md_working_2.dat","contactMatrix.md_working_2.datc1","contactMatrix.md_working_2.datc1","red")'>c1</b><span style="display:none;" id="contactMatrix.md_working_2.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=1-7 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=2.6 NN=6 MM=12}
<span style="color:blue" class="comment"># Calculate the coordination numbers for the first seven atoms in the system</span>
<span id="contactMatrix.md_working_2.datones_short"><b name="contactMatrix.md_working_2.datones" onclick='showPath("contactMatrix.md_working_2.dat","contactMatrix.md_working_2.datones","contactMatrix.md_working_2.datones_shortcut","blue")'>ones</b><span style="display:none;" id="contactMatrix.md_working_2.datones_shortcut">The ONES action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_2.datones");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=7
</span><span id="contactMatrix.md_working_2.datones_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("contactMatrix.md_working_2.datones")'># ones: ONES SIZE=7</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="contactMatrix.md_working_2.datones" onclick='showPath("contactMatrix.md_working_2.dat","contactMatrix.md_working_2.datones","contactMatrix.md_working_2.datones","blue")'>ones</b><span style="display:none;" id="contactMatrix.md_working_2.datones">The CONSTANT action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><b name="contactMatrix.md_working_2.datcc" onclick='showPath("contactMatrix.md_working_2.dat","contactMatrix.md_working_2.datcc","contactMatrix.md_working_2.datcc","blue")'>cc</b><span style="display:none;" id="contactMatrix.md_working_2.datcc">The MATRIX_VECTOR_PRODUCT action with label <b>cc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_2.datc1">c1</b>,<b name="contactMatrix.md_working_2.datones">ones</b>
<span style="color:blue" class="comment"># Set the ith element of the vector mtc equal to one if the coordination number of atom i is greater than 3.</span>
<b name="contactMatrix.md_working_2.datmtc" onclick='showPath("contactMatrix.md_working_2.dat","contactMatrix.md_working_2.datmtc","contactMatrix.md_working_2.datmtc","blue")'>mtc</b><span style="display:none;" id="contactMatrix.md_working_2.datmtc">The MORE_THAN action with label <b>mtc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mtc</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_2.datcc">cc</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL D_0=3 R_0=1}
<span style="color:blue" class="comment"># Calculate the number of atoms with a coordination number greater than 3.</span>
<b name="contactMatrix.md_working_2.dats" onclick='showPath("contactMatrix.md_working_2.dat","contactMatrix.md_working_2.dats","contactMatrix.md_working_2.dats","black")'>s</b><span style="display:none;" id="contactMatrix.md_working_2.dats">The SUM action with label <b>s</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">s</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_2.datmtc">mtc</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<span style="color:blue" class="comment"># Add a bias on s that is equal to the value of s</span>
<div class="tooltip" style="color:green">BIASVALUE<div class="right">Takes the value of one variable and use it as a bias <a href="https://www.plumed.org/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalar/vector arguments whose values will be used as a bias on the system<i></i></div></div>=<b name="contactMatrix.md_working_2.dats">s</b>
</pre>
 {% endraw %} 

for example, the diagram showing how data passes through the PLUMED actions as the values and derivatives are calculated is as follows:

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
cc(["label=cc 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subc1_mat fill:lightblue
mtc(["label=mtc 
 MORE_THAN 
"])
s(["label=s 
 SUM 
"])
end
ones(["label=ones 
 CONSTANT 
"])
c1 -- c1 --> cc
linkStyle 2 stroke:red,color:red;
ones -- ones --> cc
linkStyle 3 stroke:blue,color:blue;
cc -- cc --> mtc
linkStyle 4 stroke:blue,color:blue;
mtc -- mtc --> s
linkStyle 5 stroke:blue,color:blue;
s -- s --> 9
9(["label=#64;9 
 BIASVALUE 
"])

```
{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_contactMatrix.md_working_3.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="contactMatrix.md_working_3.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="contactMatrix.md_working_3.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Calculate the contact matrix for the first seven atoms in the system</span>
<b name="contactMatrix.md_working_3.datc1" onclick='showPath("contactMatrix.md_working_3.dat","contactMatrix.md_working_3.datc1","contactMatrix.md_working_3.datc1","red")'>c1</b><span style="display:none;" id="contactMatrix.md_working_3.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=1-7 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=2.6 NN=6 MM=12}
<span style="color:blue" class="comment"># Calculate the coordination numbers for the first seven atoms in the system</span>
<span id="contactMatrix.md_working_3.datones_short"><b name="contactMatrix.md_working_3.datones" onclick='showPath("contactMatrix.md_working_3.dat","contactMatrix.md_working_3.datones","contactMatrix.md_working_3.datones_shortcut","blue")'>ones</b><span style="display:none;" id="contactMatrix.md_working_3.datones_shortcut">The ONES action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_3.datones");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=7
</span><span id="contactMatrix.md_working_3.datones_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("contactMatrix.md_working_3.datones")'># ones: ONES SIZE=7</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="contactMatrix.md_working_3.datones" onclick='showPath("contactMatrix.md_working_3.dat","contactMatrix.md_working_3.datones","contactMatrix.md_working_3.datones","blue")'>ones</b><span style="display:none;" id="contactMatrix.md_working_3.datones">The CONSTANT action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><b name="contactMatrix.md_working_3.datcc" onclick='showPath("contactMatrix.md_working_3.dat","contactMatrix.md_working_3.datcc","contactMatrix.md_working_3.datcc","blue")'>cc</b><span style="display:none;" id="contactMatrix.md_working_3.datcc">The MATRIX_VECTOR_PRODUCT action with label <b>cc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_3.datc1">c1</b>,<b name="contactMatrix.md_working_3.datones">ones</b>
<span style="color:blue" class="comment"># Set the ith element of the vector mtc equal to one if the coordination number of atom i is greater than 3.</span>
<b name="contactMatrix.md_working_3.datmtc" onclick='showPath("contactMatrix.md_working_3.dat","contactMatrix.md_working_3.datmtc","contactMatrix.md_working_3.datmtc","blue")'>mtc</b><span style="display:none;" id="contactMatrix.md_working_3.datmtc">The MORE_THAN action with label <b>mtc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mtc</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_3.datcc">cc</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL D_0=3 R_0=1}
<span style="color:blue" class="comment"># Calculate the number of atoms with a coordination number greater than 3.</span>
<b name="contactMatrix.md_working_3.dats" onclick='showPath("contactMatrix.md_working_3.dat","contactMatrix.md_working_3.dats","contactMatrix.md_working_3.dats","black")'>s</b><span style="display:none;" id="contactMatrix.md_working_3.dats">The SUM action with label <b>s</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">s</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_3.datmtc">mtc</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<span style="color:blue" class="comment"># Add a bias on s that is equal to the value of s</span>
<div class="tooltip" style="color:green">BIASVALUE<div class="right">Takes the value of one variable and use it as a bias <a href="https://www.plumed.org/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalar/vector arguments whose values will be used as a bias on the system<i></i></div></div>=<b name="contactMatrix.md_working_3.dats">s</b>
</pre>
 {% endraw %} 

Notice that the CONTACT_MATRIX, MATRIX_VECTOR_PRODUCT, MORE_THAN and SUM actions are all in the same subgraph.  The grouping of these actions indicates that the 
first row of the contact matrix is calculated at the same time as the first elements of the vectors with labels cc and mtc.  In other words, PLUMED only starts calculating 
the second row of the matrix with label c1 once the first element of the vector mtc has been added to the scalar s.  Furthermore, the derivatives of s with respect to the 
atoms input to c1 are accumulated during the forward loop.  Consequently, when the forces from the biasvalue are applied on s they are passed through the actions as shown below:

```mermaid
flowchart BT 
9(["label=#64;9 
 BIASVALUE 
"])
9 -- s --> s
subgraph subc1 [c1]
subgraph subc1_mat [c1]
c1(["label=c1 
 CONTACT_MATRIX 
"])
cc(["label=cc 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subc1_mat fill:lightblue
c1 -. c1 .-> cc
linkStyle 1 stroke:red,color:red;
mtc(["label=mtc 
 MORE_THAN 
"])
cc -. cc .-> mtc
linkStyle 2 stroke:blue,color:blue;
s(["label=s 
 SUM 
"])
mtc -. mtc .-> s
linkStyle 3 stroke:blue,color:blue;
end
s == s ==> c1
s == s ==> cc
subgraph subc1 [c1]
end
cc -- ones --> ones
linkStyle 6 stroke:blue,color:blue;
Box("label=Box 
 PBC 
")
c1 -- Box --> Box
linkStyle 7 stroke:red,color:red;
c1 --> MD
linkStyle 8 stroke:violet,color:violet;
MD(positions from MD)

```
{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_contactMatrix.md_working_4.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="contactMatrix.md_working_4.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="contactMatrix.md_working_4.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Calculate the contact matrix for the first seven atoms in the system</span>
<b name="contactMatrix.md_working_4.datc1" onclick='showPath("contactMatrix.md_working_4.dat","contactMatrix.md_working_4.datc1","contactMatrix.md_working_4.datc1","red")'>c1</b><span style="display:none;" id="contactMatrix.md_working_4.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=1-7 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=2.6 NN=6 MM=12}
<span style="color:blue" class="comment"># Calculate the coordination numbers for the first seven atoms in the system</span>
<span id="contactMatrix.md_working_4.datones_short"><b name="contactMatrix.md_working_4.datones" onclick='showPath("contactMatrix.md_working_4.dat","contactMatrix.md_working_4.datones","contactMatrix.md_working_4.datones_shortcut","blue")'>ones</b><span style="display:none;" id="contactMatrix.md_working_4.datones_shortcut">The ONES action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_4.datones");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=7
</span><span id="contactMatrix.md_working_4.datones_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("contactMatrix.md_working_4.datones")'># ones: ONES SIZE=7</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="contactMatrix.md_working_4.datones" onclick='showPath("contactMatrix.md_working_4.dat","contactMatrix.md_working_4.datones","contactMatrix.md_working_4.datones","blue")'>ones</b><span style="display:none;" id="contactMatrix.md_working_4.datones">The CONSTANT action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><b name="contactMatrix.md_working_4.datcc" onclick='showPath("contactMatrix.md_working_4.dat","contactMatrix.md_working_4.datcc","contactMatrix.md_working_4.datcc","blue")'>cc</b><span style="display:none;" id="contactMatrix.md_working_4.datcc">The MATRIX_VECTOR_PRODUCT action with label <b>cc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_4.datc1">c1</b>,<b name="contactMatrix.md_working_4.datones">ones</b>
<span style="color:blue" class="comment"># Set the ith element of the vector mtc equal to one if the coordination number of atom i is greater than 3.</span>
<b name="contactMatrix.md_working_4.datmtc" onclick='showPath("contactMatrix.md_working_4.dat","contactMatrix.md_working_4.datmtc","contactMatrix.md_working_4.datmtc","blue")'>mtc</b><span style="display:none;" id="contactMatrix.md_working_4.datmtc">The MORE_THAN action with label <b>mtc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mtc</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_4.datcc">cc</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL D_0=3 R_0=1}
<span style="color:blue" class="comment"># Calculate the number of atoms with a coordination number greater than 3.</span>
<b name="contactMatrix.md_working_4.dats" onclick='showPath("contactMatrix.md_working_4.dat","contactMatrix.md_working_4.dats","contactMatrix.md_working_4.dats","black")'>s</b><span style="display:none;" id="contactMatrix.md_working_4.dats">The SUM action with label <b>s</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">s</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_4.datmtc">mtc</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<span style="color:blue" class="comment"># Add a bias on s that is equal to the value of s</span>
<div class="tooltip" style="color:green">BIASVALUE<div class="right">Takes the value of one variable and use it as a bias <a href="https://www.plumed.org/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalar/vector arguments whose values will be used as a bias on the system<i></i></div></div>=<b name="contactMatrix.md_working_4.dats">s</b>
</pre>
 {% endraw %} 

In short, we do not need to calculate the matrix elements of c1 twice in order to apply the forces as we accumulate the derivatives of the final scalar s during the forward loop.

## Optimisation details

The contact matrix is sparse.  Each atom is only be connected to a small number of neighbours and the vast majority of the elements of the contact matrix are thus zero.  To reduce 
the amount of memory that PLUMED requires I have thus implemented sparse matrix storage.  If you do calculate and store a contact matrix only the elements of the matrix that are 
non-zero are stored.

We can also use the sparsity of the contact matrix to make the time required to compute a contact matrix scale linearly rather than quadratically with the number of atoms.  Element 
$i,j$ of the contact matrix is only non-zero if two atoms are within a cutoff, $r_c$.  We can determine that many pairs of atoms are further appart than $r_c$ without computing the 
distance between these atoms by using divide and conquer strategies such as linked lists and neighbour lists.  These optimisation tricks are implemented in the base class AgencyMatrixBase.  
This class therefore ensures that only the subset of elements of the contact matrix that are definitely non-zero are computed.  Furthermore, because coordination numbers are computed 
within the chain of actions only the non-zero elements of the matrix are propegated onwards through the chain when we multiply by the vector of ones.  In the flowchart diagrams that I have 
shown previously the blue subgraphs illustrate how data is passed through actions as the elements of the matrix row are evaluated.

## A complicated CV

Consider the CV that was used to study perovskite nucleation in [this paper](https://pubs.acs.org/doi/abs/10.1021/acs.chemmater.9b04259).  The CV here measures the number of 
methylamonium molecules that are attached to at least 5 other methylamoniusm molecules, at least 7 lead atoms and at least 11 ionide ions.  We can calculate something akin to this 
CV and apply a restraint on the resulting quantity by using the following input file:

```mermaid
flowchart BT 
rr(["label=rr 
 RESTRAINT 
"])
rr -- ff --> ff
subgraph subcm_cncn [cm_cncn]
subgraph subcm_cncn_mat [cm_cncn]
cm_cncn(["label=cm_cncn 
 CONTACT_MATRIX 
"])
cc_cncn(["label=cc_cncn 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subcm_cncn_mat fill:lightblue
cm_cncn -. cm_cncn .-> cc_cncn
linkStyle 1 stroke:red,color:red;
mt_cncn(["label=mt_cncn 
 MORE_THAN 
"])
cc_cncn -. cc_cncn .-> mt_cncn
linkStyle 2 stroke:blue,color:blue;
subgraph subcm_cnpb_mat [cm_cnpb]
cm_cnpb(["label=cm_cnpb 
 CONTACT_MATRIX 
"])
cc_cnpb(["label=cc_cnpb 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subcm_cnpb_mat fill:lightblue
cm_cnpb -. cm_cnpb .-> cc_cnpb
linkStyle 3 stroke:red,color:red;
mt_cnpb(["label=mt_cnpb 
 MORE_THAN 
"])
cc_cnpb -. cc_cnpb .-> mt_cnpb
linkStyle 4 stroke:blue,color:blue;
subgraph subcm_cnI_mat [cm_cnI]
cm_cnI(["label=cm_cnI 
 CONTACT_MATRIX 
"])
cc_cnI(["label=cc_cnI 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subcm_cnI_mat fill:lightblue
cm_cnI -. cm_cnI .-> cc_cnI
linkStyle 5 stroke:red,color:red;
mt_cnI(["label=mt_cnI 
 MORE_THAN 
"])
cc_cnI -. cc_cnI .-> mt_cnI
linkStyle 6 stroke:blue,color:blue;
mm(["label=mm 
 CUSTOM
FUNC=x*y*z 
"])
mt_cncn -. mt_cncn .-> mm
linkStyle 7 stroke:blue,color:blue;
mt_cnpb -. mt_cnpb .-> mm
linkStyle 8 stroke:blue,color:blue;
mt_cnI -. mt_cnI .-> mm
linkStyle 9 stroke:blue,color:blue;
ff(["label=ff 
 SUM 
"])
mm -. mm .-> ff
linkStyle 10 stroke:blue,color:blue;
end
ff == ff ==> cm_cncn
ff == ff ==> cc_cncn
ff == ff ==> cm_cnpb
ff == ff ==> cc_cnpb
ff == ff ==> cm_cnI
ff == ff ==> cc_cnI
subgraph subcm_cncn [cm_cncn]
end
cc_cnI -- ones192 --> ones192
linkStyle 17 stroke:blue,color:blue;
subgraph subcm_cncn [cm_cncn]
end
cc_cnpb -- ones64 --> ones64
linkStyle 18 stroke:blue,color:blue;
subgraph subcm_cncn [cm_cncn]
end
cc_cncn -- ones64 --> ones64
linkStyle 19 stroke:blue,color:blue;
Box("label=Box 
 PBC 
")
cm_cnI -- Box --> Box
linkStyle 20 stroke:red,color:red;
cm_cnI --> MD
linkStyle 21 stroke:violet,color:violet;
cm_cncn -- Box --> Box
linkStyle 22 stroke:red,color:red;
cm_cncn --> MD
linkStyle 23 stroke:violet,color:violet;
cm_cnpb -- Box --> Box
linkStyle 24 stroke:red,color:red;
cm_cnpb --> MD
linkStyle 25 stroke:violet,color:violet;
MD(positions from MD)

```
{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_contactMatrix.md_working_5.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="contactMatrix.md_working_5.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="contactMatrix.md_working_5.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Lead ions</span>
<b name="contactMatrix.md_working_5.datPb" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datPb","contactMatrix.md_working_5.datPb","violet")'>Pb</b><span style="display:none;" id="contactMatrix.md_working_5.datPb">The GROUP action with label <b>Pb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">Pb</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=1-64
<span style="color:blue" class="comment"># Iodide atoms</span>
<b name="contactMatrix.md_working_5.datI" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datI","contactMatrix.md_working_5.datI","violet")'>I</b><span style="display:none;" id="contactMatrix.md_working_5.datI">The GROUP action with label <b>I</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">I</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=65-256  
<span style="color:blue" class="comment"># Methylamonium &quot;atoms&quot; -- in the real CV these are centers of mass rather than single atoms</span>
<b name="contactMatrix.md_working_5.datcn" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datcn","contactMatrix.md_working_5.datcn","violet")'>cn</b><span style="display:none;" id="contactMatrix.md_working_5.datcn">The GROUP action with label <b>cn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cn</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=257-320
<br/><span id="contactMatrix.md_working_5.datones64_short"><b name="contactMatrix.md_working_5.datones64" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datones64","contactMatrix.md_working_5.datones64_shortcut","blue")'>ones64</b><span style="display:none;" id="contactMatrix.md_working_5.datones64_shortcut">The ONES action with label <b>ones64</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones64</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_5.datones64");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=64
</span><span id="contactMatrix.md_working_5.datones64_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("contactMatrix.md_working_5.datones64")'># ones64: ONES SIZE=64</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="contactMatrix.md_working_5.datones64" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datones64","contactMatrix.md_working_5.datones64","blue")'>ones64</b><span style="display:none;" id="contactMatrix.md_working_5.datones64">The CONSTANT action with label <b>ones64</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones64</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><span style="color:blue" class="comment"># Contact matrix that determines if methylamonium molecules are within 8 A of each other</span>
<b name="contactMatrix.md_working_5.datcm_cncn" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datcm_cncn","contactMatrix.md_working_5.datcm_cncn","red")'>cm_cncn</b><span style="display:none;" id="contactMatrix.md_working_5.datcm_cncn">The CONTACT_MATRIX action with label <b>cm_cncn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cm_cncn</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=<b name="contactMatrix.md_working_5.datcn">cn</b> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.8}
<span style="color:blue" class="comment"># Coordination number of methylamounium with methylamonium</span>
<b name="contactMatrix.md_working_5.datcc_cncn" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datcc_cncn","contactMatrix.md_working_5.datcc_cncn","blue")'>cc_cncn</b><span style="display:none;" id="contactMatrix.md_working_5.datcc_cncn">The MATRIX_VECTOR_PRODUCT action with label <b>cc_cncn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc_cncn</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_5.datcm_cncn">cm_cncn</b>,<b name="contactMatrix.md_working_5.datones64">ones64</b>
<span style="color:blue" class="comment"># Vector with elements that are one if coordiantion of methylamonium with methylamonium &gt;5</span>
<b name="contactMatrix.md_working_5.datmt_cncn" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datmt_cncn","contactMatrix.md_working_5.datmt_cncn","blue")'>mt_cncn</b><span style="display:none;" id="contactMatrix.md_working_5.datmt_cncn">The MORE_THAN action with label <b>mt_cncn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt_cncn</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_5.datcc_cncn">cc_cncn</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=5 NN=12 MM=24}
<br/><span style="color:blue" class="comment"># Contact matrix that determines if methylamoinium moleulcule and Pb atom are within 7.5 A of each other</span>
<b name="contactMatrix.md_working_5.datcm_cnpb" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datcm_cnpb","contactMatrix.md_working_5.datcm_cnpb","red")'>cm_cnpb</b><span style="display:none;" id="contactMatrix.md_working_5.datcm_cnpb">The CONTACT_MATRIX action with label <b>cm_cnpb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cm_cnpb</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUPA=<b name="contactMatrix.md_working_5.datcn">cn</b> GROUPB=<b name="contactMatrix.md_working_5.datPb">Pb</b> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.75}
<span style="color:blue" class="comment"># Coordination number of methylamonium with Pb</span>
<b name="contactMatrix.md_working_5.datcc_cnpb" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datcc_cnpb","contactMatrix.md_working_5.datcc_cnpb","blue")'>cc_cnpb</b><span style="display:none;" id="contactMatrix.md_working_5.datcc_cnpb">The MATRIX_VECTOR_PRODUCT action with label <b>cc_cnpb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc_cnpb</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_5.datcm_cnpb">cm_cnpb</b>,<b name="contactMatrix.md_working_5.datones64">ones64</b>
<span style="color:blue" class="comment"># Vector with elements that are one if coordination of methylamounium with lead is &gt;7</span>
<b name="contactMatrix.md_working_5.datmt_cnpb" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datmt_cnpb","contactMatrix.md_working_5.datmt_cnpb","blue")'>mt_cnpb</b><span style="display:none;" id="contactMatrix.md_working_5.datmt_cnpb">The MORE_THAN action with label <b>mt_cnpb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt_cnpb</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_5.datcc_cnpb">cc_cnpb</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=7 NN=12 MM=24}
<br/><span id="contactMatrix.md_working_5.datones192_short"><b name="contactMatrix.md_working_5.datones192" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datones192","contactMatrix.md_working_5.datones192_shortcut","blue")'>ones192</b><span style="display:none;" id="contactMatrix.md_working_5.datones192_shortcut">The ONES action with label <b>ones192</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones192</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_5.datones192");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=192
</span><span id="contactMatrix.md_working_5.datones192_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("contactMatrix.md_working_5.datones192")'># ones192: ONES SIZE=192</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="contactMatrix.md_working_5.datones192" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datones192","contactMatrix.md_working_5.datones192","blue")'>ones192</b><span style="display:none;" id="contactMatrix.md_working_5.datones192">The CONSTANT action with label <b>ones192</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones192</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><span style="color:blue" class="comment"># Contact matrix that determines if methylamoinium moleulcule and I atom are within 6.5 A of each other</span>
<b name="contactMatrix.md_working_5.datcm_cnI" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datcm_cnI","contactMatrix.md_working_5.datcm_cnI","red")'>cm_cnI</b><span style="display:none;" id="contactMatrix.md_working_5.datcm_cnI">The CONTACT_MATRIX action with label <b>cm_cnI</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cm_cnI</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUPA=<b name="contactMatrix.md_working_5.datcn">cn</b> GROUPB=<b name="contactMatrix.md_working_5.datI">I</b> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.65}
<span style="color:blue" class="comment"># Coordination number of methylamonium with I</span>
<b name="contactMatrix.md_working_5.datcc_cnI" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datcc_cnI","contactMatrix.md_working_5.datcc_cnI","blue")'>cc_cnI</b><span style="display:none;" id="contactMatrix.md_working_5.datcc_cnI">The MATRIX_VECTOR_PRODUCT action with label <b>cc_cnI</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc_cnI</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_5.datcm_cnI">cm_cnI</b>,<b name="contactMatrix.md_working_5.datones192">ones192</b>
<span style="color:blue" class="comment"># Vector with elements that are one if coordination of methylamounium with lead is &gt;11</span>
<b name="contactMatrix.md_working_5.datmt_cnI" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datmt_cnI","contactMatrix.md_working_5.datmt_cnI","blue")'>mt_cnI</b><span style="display:none;" id="contactMatrix.md_working_5.datmt_cnI">The MORE_THAN action with label <b>mt_cnI</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt_cnI</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_5.datcc_cnI">cc_cnI</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=11 NN=12 MM=24}
<br/><span style="color:blue" class="comment"># Element wise product of these three input vectors.</span>
<span style="color:blue" class="comment"># mm[i]==1 if coordination number of corrsponding methylamounium with methylamonium is &gt;5</span>
<span style="color:blue" class="comment"># and if coordination of methylamounium with Pb is &gt;7 and if coordination of methylamounium with I &gt; 11</span>
<b name="contactMatrix.md_working_5.datmm" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datmm","contactMatrix.md_working_5.datmm","blue")'>mm</b><span style="display:none;" id="contactMatrix.md_working_5.datmm">The CUSTOM action with label <b>mm</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mm</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of an arbitrary function to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_5.datmt_cncn">mt_cncn</b>,<b name="contactMatrix.md_working_5.datmt_cnpb">mt_cnpb</b>,<b name="contactMatrix.md_working_5.datmt_cnI">mt_cnI</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=x*y*z <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<br/><span style="color:blue" class="comment"># Sum of coordination numbers and thus equal to number of methylamoniums with desired coordination numbers</span>
<b name="contactMatrix.md_working_5.datff" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datff","contactMatrix.md_working_5.datff","black")'>ff</b><span style="display:none;" id="contactMatrix.md_working_5.datff">The SUM action with label <b>ff</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ff</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_5.datmm">mm</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<br/><span id="contactMatrix.md_working_5.datdefrr_short"><b name="contactMatrix.md_working_5.datrr" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datrr","contactMatrix.md_working_5.datrr","black")'>rr</b><span style="display:none;" id="contactMatrix.md_working_5.datrr">The RESTRAINT action with label <b>rr</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">rr.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">rr.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_5.datdefrr");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="contactMatrix.md_working_5.datff">ff</b> <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=62 <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=10
</span><span id="contactMatrix.md_working_5.datdefrr_long" style="display:none;"><b name="contactMatrix.md_working_5.datrr" onclick='showPath("contactMatrix.md_working_5.dat","contactMatrix.md_working_5.datrr","contactMatrix.md_working_5.datrr","black")'>rr</b>: <div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_5.datdefrr");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="contactMatrix.md_working_5.datff">ff</b> <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=62 <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=10  <div class="tooltip">SLOPE<div class="right"> specifies that the restraint is linear and what the values of the force constants on each of the variables are<i></i></div></div>=0.0
</span></pre>
 {% endraw %} 

When the forward loop through the actions in the above input file is performed data is passed as follows:

```mermaid
flowchart TB 
MD(positions from MD)
Box("label=Box 
 PBC 
")
Pb("label=Pb 
 GROUP 
")
I("label=I 
 GROUP 
")
cn("label=cn 
 GROUP 
")
ones64(["label=ones64 
 CONSTANT 
"])
Box -- Box --> cm_cncn
linkStyle 0 stroke:red,color:red;
MD --> cm_cncn
linkStyle 1 stroke:violet,color:violet;
subgraph subcm_cncn [cm_cncn]
subgraph subcm_cncn_mat [cm_cncn]
cm_cncn(["label=cm_cncn 
 CONTACT_MATRIX 
"])
cc_cncn(["label=cc_cncn 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subcm_cncn_mat fill:lightblue
mt_cncn(["label=mt_cncn 
 MORE_THAN 
"])
subgraph subcm_cnpb_mat [cm_cnpb]
cm_cnpb(["label=cm_cnpb 
 CONTACT_MATRIX 
"])
cc_cnpb(["label=cc_cnpb 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subcm_cnpb_mat fill:lightblue
mt_cnpb(["label=mt_cnpb 
 MORE_THAN 
"])
subgraph subcm_cnI_mat [cm_cnI]
cm_cnI(["label=cm_cnI 
 CONTACT_MATRIX 
"])
cc_cnI(["label=cc_cnI 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subcm_cnI_mat fill:lightblue
mt_cnI(["label=mt_cnI 
 MORE_THAN 
"])
mm(["label=mm 
 CUSTOM
FUNC=x*y*z 
"])
ff(["label=ff 
 SUM 
"])
end
cm_cncn -- cm_cncn --> cc_cncn
linkStyle 2 stroke:red,color:red;
ones64 -- ones64 --> cc_cncn
linkStyle 3 stroke:blue,color:blue;
cc_cncn -- cc_cncn --> mt_cncn
linkStyle 4 stroke:blue,color:blue;
Box -- Box --> cm_cnpb
linkStyle 5 stroke:red,color:red;
MD --> cm_cnpb
linkStyle 6 stroke:violet,color:violet;
cm_cnpb -- cm_cnpb --> cc_cnpb
linkStyle 7 stroke:red,color:red;
ones64 -- ones64 --> cc_cnpb
linkStyle 8 stroke:blue,color:blue;
cc_cnpb -- cc_cnpb --> mt_cnpb
linkStyle 9 stroke:blue,color:blue;
ones192(["label=ones192 
 CONSTANT 
"])
Box -- Box --> cm_cnI
linkStyle 10 stroke:red,color:red;
MD --> cm_cnI
linkStyle 11 stroke:violet,color:violet;
cm_cnI -- cm_cnI --> cc_cnI
linkStyle 12 stroke:red,color:red;
ones192 -- ones192 --> cc_cnI
linkStyle 13 stroke:blue,color:blue;
cc_cnI -- cc_cnI --> mt_cnI
linkStyle 14 stroke:blue,color:blue;
mt_cncn -- mt_cncn --> mm
linkStyle 15 stroke:blue,color:blue;
mt_cnpb -- mt_cnpb --> mm
linkStyle 16 stroke:blue,color:blue;
mt_cnI -- mt_cnI --> mm
linkStyle 17 stroke:blue,color:blue;
mm -- mm --> ff
linkStyle 18 stroke:blue,color:blue;
ff -- ff --> rr
rr(["label=rr 
 RESTRAINT 
"])

```
{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_contactMatrix.md_working_6.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="contactMatrix.md_working_6.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="contactMatrix.md_working_6.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Lead ions</span>
<b name="contactMatrix.md_working_6.datPb" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datPb","contactMatrix.md_working_6.datPb","violet")'>Pb</b><span style="display:none;" id="contactMatrix.md_working_6.datPb">The GROUP action with label <b>Pb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">Pb</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=1-64
<span style="color:blue" class="comment"># Iodide atoms</span>
<b name="contactMatrix.md_working_6.datI" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datI","contactMatrix.md_working_6.datI","violet")'>I</b><span style="display:none;" id="contactMatrix.md_working_6.datI">The GROUP action with label <b>I</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">I</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=65-256
<span style="color:blue" class="comment"># Methylamonium &quot;atoms&quot; -- in the real CV these are centers of mass rather than single atoms</span>
<b name="contactMatrix.md_working_6.datcn" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datcn","contactMatrix.md_working_6.datcn","violet")'>cn</b><span style="display:none;" id="contactMatrix.md_working_6.datcn">The GROUP action with label <b>cn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cn</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=257-320
<br/><span id="contactMatrix.md_working_6.datones64_short"><b name="contactMatrix.md_working_6.datones64" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datones64","contactMatrix.md_working_6.datones64_shortcut","blue")'>ones64</b><span style="display:none;" id="contactMatrix.md_working_6.datones64_shortcut">The ONES action with label <b>ones64</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones64</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_6.datones64");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=64
</span><span id="contactMatrix.md_working_6.datones64_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("contactMatrix.md_working_6.datones64")'># ones64: ONES SIZE=64</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="contactMatrix.md_working_6.datones64" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datones64","contactMatrix.md_working_6.datones64","blue")'>ones64</b><span style="display:none;" id="contactMatrix.md_working_6.datones64">The CONSTANT action with label <b>ones64</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones64</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><span style="color:blue" class="comment"># Contact matrix that determines if methylamonium molecules are within 8 A of each other</span>
<b name="contactMatrix.md_working_6.datcm_cncn" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datcm_cncn","contactMatrix.md_working_6.datcm_cncn","red")'>cm_cncn</b><span style="display:none;" id="contactMatrix.md_working_6.datcm_cncn">The CONTACT_MATRIX action with label <b>cm_cncn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cm_cncn</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=<b name="contactMatrix.md_working_6.datcn">cn</b> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.8}
<span style="color:blue" class="comment"># Coordination number of methylamounium with methylamonium</span>
<b name="contactMatrix.md_working_6.datcc_cncn" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datcc_cncn","contactMatrix.md_working_6.datcc_cncn","blue")'>cc_cncn</b><span style="display:none;" id="contactMatrix.md_working_6.datcc_cncn">The MATRIX_VECTOR_PRODUCT action with label <b>cc_cncn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc_cncn</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_6.datcm_cncn">cm_cncn</b>,<b name="contactMatrix.md_working_6.datones64">ones64</b>
<span style="color:blue" class="comment"># Vector with elements that are one if coordiantion of methylamonium with methylamonium &gt;5</span>
<b name="contactMatrix.md_working_6.datmt_cncn" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datmt_cncn","contactMatrix.md_working_6.datmt_cncn","blue")'>mt_cncn</b><span style="display:none;" id="contactMatrix.md_working_6.datmt_cncn">The MORE_THAN action with label <b>mt_cncn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt_cncn</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_6.datcc_cncn">cc_cncn</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=5 NN=12 MM=24}
<br/><span style="color:blue" class="comment"># Contact matrix that determines if methylamoinium moleulcule and Pb atom are within 7.5 A of each other</span>
<b name="contactMatrix.md_working_6.datcm_cnpb" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datcm_cnpb","contactMatrix.md_working_6.datcm_cnpb","red")'>cm_cnpb</b><span style="display:none;" id="contactMatrix.md_working_6.datcm_cnpb">The CONTACT_MATRIX action with label <b>cm_cnpb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cm_cnpb</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUPA=<b name="contactMatrix.md_working_6.datcn">cn</b> GROUPB=<b name="contactMatrix.md_working_6.datPb">Pb</b> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.75}
<span style="color:blue" class="comment"># Coordination number of methylamonium with Pb</span>
<b name="contactMatrix.md_working_6.datcc_cnpb" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datcc_cnpb","contactMatrix.md_working_6.datcc_cnpb","blue")'>cc_cnpb</b><span style="display:none;" id="contactMatrix.md_working_6.datcc_cnpb">The MATRIX_VECTOR_PRODUCT action with label <b>cc_cnpb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc_cnpb</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_6.datcm_cnpb">cm_cnpb</b>,<b name="contactMatrix.md_working_6.datones64">ones64</b>
<span style="color:blue" class="comment"># Vector with elements that are one if coordination of methylamounium with lead is &gt;7</span>
<b name="contactMatrix.md_working_6.datmt_cnpb" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datmt_cnpb","contactMatrix.md_working_6.datmt_cnpb","blue")'>mt_cnpb</b><span style="display:none;" id="contactMatrix.md_working_6.datmt_cnpb">The MORE_THAN action with label <b>mt_cnpb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt_cnpb</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_6.datcc_cnpb">cc_cnpb</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=7 NN=12 MM=24}
<br/><span id="contactMatrix.md_working_6.datones192_short"><b name="contactMatrix.md_working_6.datones192" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datones192","contactMatrix.md_working_6.datones192_shortcut","blue")'>ones192</b><span style="display:none;" id="contactMatrix.md_working_6.datones192_shortcut">The ONES action with label <b>ones192</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones192</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_6.datones192");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=192
</span><span id="contactMatrix.md_working_6.datones192_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("contactMatrix.md_working_6.datones192")'># ones192: ONES SIZE=192</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="contactMatrix.md_working_6.datones192" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datones192","contactMatrix.md_working_6.datones192","blue")'>ones192</b><span style="display:none;" id="contactMatrix.md_working_6.datones192">The CONSTANT action with label <b>ones192</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones192</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><span style="color:blue" class="comment"># Contact matrix that determines if methylamoinium moleulcule and I atom are within 6.5 A of each other</span>
<b name="contactMatrix.md_working_6.datcm_cnI" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datcm_cnI","contactMatrix.md_working_6.datcm_cnI","red")'>cm_cnI</b><span style="display:none;" id="contactMatrix.md_working_6.datcm_cnI">The CONTACT_MATRIX action with label <b>cm_cnI</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cm_cnI</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUPA=<b name="contactMatrix.md_working_6.datcn">cn</b> GROUPB=<b name="contactMatrix.md_working_6.datI">I</b> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.65}
<span style="color:blue" class="comment"># Coordination number of methylamonium with I</span>
<b name="contactMatrix.md_working_6.datcc_cnI" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datcc_cnI","contactMatrix.md_working_6.datcc_cnI","blue")'>cc_cnI</b><span style="display:none;" id="contactMatrix.md_working_6.datcc_cnI">The MATRIX_VECTOR_PRODUCT action with label <b>cc_cnI</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc_cnI</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_6.datcm_cnI">cm_cnI</b>,<b name="contactMatrix.md_working_6.datones192">ones192</b>
<span style="color:blue" class="comment"># Vector with elements that are one if coordination of methylamounium with lead is &gt;11</span>
<b name="contactMatrix.md_working_6.datmt_cnI" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datmt_cnI","contactMatrix.md_working_6.datmt_cnI","blue")'>mt_cnI</b><span style="display:none;" id="contactMatrix.md_working_6.datmt_cnI">The MORE_THAN action with label <b>mt_cnI</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt_cnI</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_6.datcc_cnI">cc_cnI</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=11 NN=12 MM=24}
<br/><span style="color:blue" class="comment"># Element wise product of these three input vectors.</span>
<span style="color:blue" class="comment"># mm[i]==1 if coordination number of corrsponding methylamounium with methylamonium is &gt;5</span>
<span style="color:blue" class="comment"># and if coordination of methylamounium with Pb is &gt;7 and if coordination of methylamounium with I &gt; 11</span>
<b name="contactMatrix.md_working_6.datmm" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datmm","contactMatrix.md_working_6.datmm","blue")'>mm</b><span style="display:none;" id="contactMatrix.md_working_6.datmm">The CUSTOM action with label <b>mm</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mm</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of an arbitrary function to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_6.datmt_cncn">mt_cncn</b>,<b name="contactMatrix.md_working_6.datmt_cnpb">mt_cnpb</b>,<b name="contactMatrix.md_working_6.datmt_cnI">mt_cnI</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=x*y*z <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<br/><span style="color:blue" class="comment"># Sum of coordination numbers and thus equal to number of methylamoniums with desired coordination numbers</span>
<b name="contactMatrix.md_working_6.datff" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datff","contactMatrix.md_working_6.datff","black")'>ff</b><span style="display:none;" id="contactMatrix.md_working_6.datff">The SUM action with label <b>ff</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ff</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_6.datmm">mm</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<br/><span id="contactMatrix.md_working_6.datdefrr_short"><b name="contactMatrix.md_working_6.datrr" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datrr","contactMatrix.md_working_6.datrr","black")'>rr</b><span style="display:none;" id="contactMatrix.md_working_6.datrr">The RESTRAINT action with label <b>rr</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">rr.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">rr.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_6.datdefrr");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="contactMatrix.md_working_6.datff">ff</b> <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=62 <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=10
</span><span id="contactMatrix.md_working_6.datdefrr_long" style="display:none;"><b name="contactMatrix.md_working_6.datrr" onclick='showPath("contactMatrix.md_working_6.dat","contactMatrix.md_working_6.datrr","contactMatrix.md_working_6.datrr","black")'>rr</b>: <div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_6.datdefrr");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="contactMatrix.md_working_6.datff">ff</b> <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=62 <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=10  <div class="tooltip">SLOPE<div class="right"> specifies that the restraint is linear and what the values of the force constants on each of the variables are<i></i></div></div>=0.0
</span></pre>
 {% endraw %} 

You can clearly see from this diagram that all the actions that are needed to calculate the final biased quantity ff are in the same subgraph.  We thus calculate the derivatives of ff with respect to the input 
atomic positions in the forward loop so the forces from the restraint can be passed backwards through the actions as follows:

```mermaid
flowchart BT 
rr(["label=rr 
 RESTRAINT 
"])
rr -- ff --> ff
subgraph subcm_cncn [cm_cncn]
subgraph subcm_cncn_mat [cm_cncn]
cm_cncn(["label=cm_cncn 
 CONTACT_MATRIX 
"])
cc_cncn(["label=cc_cncn 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subcm_cncn_mat fill:lightblue
cm_cncn -. cm_cncn .-> cc_cncn
linkStyle 1 stroke:red,color:red;
mt_cncn(["label=mt_cncn 
 MORE_THAN 
"])
cc_cncn -. cc_cncn .-> mt_cncn
linkStyle 2 stroke:blue,color:blue;
subgraph subcm_cnpb_mat [cm_cnpb]
cm_cnpb(["label=cm_cnpb 
 CONTACT_MATRIX 
"])
cc_cnpb(["label=cc_cnpb 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subcm_cnpb_mat fill:lightblue
cm_cnpb -. cm_cnpb .-> cc_cnpb
linkStyle 3 stroke:red,color:red;
mt_cnpb(["label=mt_cnpb 
 MORE_THAN 
"])
cc_cnpb -. cc_cnpb .-> mt_cnpb
linkStyle 4 stroke:blue,color:blue;
subgraph subcm_cnI_mat [cm_cnI]
cm_cnI(["label=cm_cnI 
 CONTACT_MATRIX 
"])
cc_cnI(["label=cc_cnI 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subcm_cnI_mat fill:lightblue
cm_cnI -. cm_cnI .-> cc_cnI
linkStyle 5 stroke:red,color:red;
mt_cnI(["label=mt_cnI 
 MORE_THAN 
"])
cc_cnI -. cc_cnI .-> mt_cnI
linkStyle 6 stroke:blue,color:blue;
mm(["label=mm 
 CUSTOM
FUNC=x*y*z 
"])
mt_cncn -. mt_cncn .-> mm
linkStyle 7 stroke:blue,color:blue;
mt_cnpb -. mt_cnpb .-> mm
linkStyle 8 stroke:blue,color:blue;
mt_cnI -. mt_cnI .-> mm
linkStyle 9 stroke:blue,color:blue;
ff(["label=ff 
 SUM 
"])
mm -. mm .-> ff
linkStyle 10 stroke:blue,color:blue;
end
ff == ff ==> cm_cncn
ff == ff ==> cc_cncn
ff == ff ==> cm_cnpb
ff == ff ==> cc_cnpb
ff == ff ==> cm_cnI
ff == ff ==> cc_cnI
subgraph subcm_cncn [cm_cncn]
end
cc_cnI -- ones192 --> ones192
linkStyle 17 stroke:blue,color:blue;
subgraph subcm_cncn [cm_cncn]
end
cc_cnpb -- ones64 --> ones64
linkStyle 18 stroke:blue,color:blue;
subgraph subcm_cncn [cm_cncn]
end
cc_cncn -- ones64 --> ones64
linkStyle 19 stroke:blue,color:blue;
Box("label=Box 
 PBC 
")
cm_cnI -- Box --> Box
linkStyle 20 stroke:red,color:red;
cm_cnI --> MD
linkStyle 21 stroke:violet,color:violet;
cm_cncn -- Box --> Box
linkStyle 22 stroke:red,color:red;
cm_cncn --> MD
linkStyle 23 stroke:violet,color:violet;
cm_cnpb -- Box --> Box
linkStyle 24 stroke:red,color:red;
cm_cnpb --> MD
linkStyle 25 stroke:violet,color:violet;
MD(positions from MD)

```
{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_contactMatrix.md_working_7.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="contactMatrix.md_working_7.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="contactMatrix.md_working_7.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Lead ions</span>
<b name="contactMatrix.md_working_7.datPb" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datPb","contactMatrix.md_working_7.datPb","violet")'>Pb</b><span style="display:none;" id="contactMatrix.md_working_7.datPb">The GROUP action with label <b>Pb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">Pb</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=1-64
<span style="color:blue" class="comment"># Iodide atoms</span>
<b name="contactMatrix.md_working_7.datI" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datI","contactMatrix.md_working_7.datI","violet")'>I</b><span style="display:none;" id="contactMatrix.md_working_7.datI">The GROUP action with label <b>I</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">I</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=65-256
<span style="color:blue" class="comment"># Methylamonium &quot;atoms&quot; -- in the real CV these are centers of mass rather than single atoms</span>
<b name="contactMatrix.md_working_7.datcn" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datcn","contactMatrix.md_working_7.datcn","violet")'>cn</b><span style="display:none;" id="contactMatrix.md_working_7.datcn">The GROUP action with label <b>cn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cn</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=257-320
<br/><span id="contactMatrix.md_working_7.datones64_short"><b name="contactMatrix.md_working_7.datones64" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datones64","contactMatrix.md_working_7.datones64_shortcut","blue")'>ones64</b><span style="display:none;" id="contactMatrix.md_working_7.datones64_shortcut">The ONES action with label <b>ones64</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones64</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_7.datones64");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=64
</span><span id="contactMatrix.md_working_7.datones64_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("contactMatrix.md_working_7.datones64")'># ones64: ONES SIZE=64</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="contactMatrix.md_working_7.datones64" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datones64","contactMatrix.md_working_7.datones64","blue")'>ones64</b><span style="display:none;" id="contactMatrix.md_working_7.datones64">The CONSTANT action with label <b>ones64</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones64</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><span style="color:blue" class="comment"># Contact matrix that determines if methylamonium molecules are within 8 A of each other</span>
<b name="contactMatrix.md_working_7.datcm_cncn" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datcm_cncn","contactMatrix.md_working_7.datcm_cncn","red")'>cm_cncn</b><span style="display:none;" id="contactMatrix.md_working_7.datcm_cncn">The CONTACT_MATRIX action with label <b>cm_cncn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cm_cncn</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">GROUP<div class="right">specifies the list of atoms that should be assumed indistinguishable<i></i></div></div>=<b name="contactMatrix.md_working_7.datcn">cn</b> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.8}
<span style="color:blue" class="comment"># Coordination number of methylamounium with methylamonium</span>
<b name="contactMatrix.md_working_7.datcc_cncn" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datcc_cncn","contactMatrix.md_working_7.datcc_cncn","blue")'>cc_cncn</b><span style="display:none;" id="contactMatrix.md_working_7.datcc_cncn">The MATRIX_VECTOR_PRODUCT action with label <b>cc_cncn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc_cncn</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_7.datcm_cncn">cm_cncn</b>,<b name="contactMatrix.md_working_7.datones64">ones64</b>
<span style="color:blue" class="comment"># Vector with elements that are one if coordiantion of methylamonium with methylamonium &gt;5</span>
<b name="contactMatrix.md_working_7.datmt_cncn" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datmt_cncn","contactMatrix.md_working_7.datmt_cncn","blue")'>mt_cncn</b><span style="display:none;" id="contactMatrix.md_working_7.datmt_cncn">The MORE_THAN action with label <b>mt_cncn</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt_cncn</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_7.datcc_cncn">cc_cncn</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=5 NN=12 MM=24}
<br/><span style="color:blue" class="comment"># Contact matrix that determines if methylamoinium moleulcule and Pb atom are within 7.5 A of each other</span>
<b name="contactMatrix.md_working_7.datcm_cnpb" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datcm_cnpb","contactMatrix.md_working_7.datcm_cnpb","red")'>cm_cnpb</b><span style="display:none;" id="contactMatrix.md_working_7.datcm_cnpb">The CONTACT_MATRIX action with label <b>cm_cnpb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cm_cnpb</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUPA=<b name="contactMatrix.md_working_7.datcn">cn</b> GROUPB=<b name="contactMatrix.md_working_7.datPb">Pb</b> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.75}
<span style="color:blue" class="comment"># Coordination number of methylamonium with Pb</span>
<b name="contactMatrix.md_working_7.datcc_cnpb" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datcc_cnpb","contactMatrix.md_working_7.datcc_cnpb","blue")'>cc_cnpb</b><span style="display:none;" id="contactMatrix.md_working_7.datcc_cnpb">The MATRIX_VECTOR_PRODUCT action with label <b>cc_cnpb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc_cnpb</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_7.datcm_cnpb">cm_cnpb</b>,<b name="contactMatrix.md_working_7.datones64">ones64</b>
<span style="color:blue" class="comment"># Vector with elements that are one if coordination of methylamounium with lead is &gt;7</span>
<b name="contactMatrix.md_working_7.datmt_cnpb" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datmt_cnpb","contactMatrix.md_working_7.datmt_cnpb","blue")'>mt_cnpb</b><span style="display:none;" id="contactMatrix.md_working_7.datmt_cnpb">The MORE_THAN action with label <b>mt_cnpb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt_cnpb</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_7.datcc_cnpb">cc_cnpb</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=7 NN=12 MM=24}
<br/><span id="contactMatrix.md_working_7.datones192_short"><b name="contactMatrix.md_working_7.datones192" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datones192","contactMatrix.md_working_7.datones192_shortcut","blue")'>ones192</b><span style="display:none;" id="contactMatrix.md_working_7.datones192_shortcut">The ONES action with label <b>ones192</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones192</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_7.datones192");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=192
</span><span id="contactMatrix.md_working_7.datones192_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("contactMatrix.md_working_7.datones192")'># ones192: ONES SIZE=192</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="contactMatrix.md_working_7.datones192" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datones192","contactMatrix.md_working_7.datones192","blue")'>ones192</b><span style="display:none;" id="contactMatrix.md_working_7.datones192">The CONSTANT action with label <b>ones192</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones192</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><span style="color:blue" class="comment"># Contact matrix that determines if methylamoinium moleulcule and I atom are within 6.5 A of each other</span>
<b name="contactMatrix.md_working_7.datcm_cnI" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datcm_cnI","contactMatrix.md_working_7.datcm_cnI","red")'>cm_cnI</b><span style="display:none;" id="contactMatrix.md_working_7.datcm_cnI">The CONTACT_MATRIX action with label <b>cm_cnI</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cm_cnI</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUPA=<b name="contactMatrix.md_working_7.datcn">cn</b> GROUPB=<b name="contactMatrix.md_working_7.datI">I</b> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.65}
<span style="color:blue" class="comment"># Coordination number of methylamonium with I</span>
<b name="contactMatrix.md_working_7.datcc_cnI" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datcc_cnI","contactMatrix.md_working_7.datcc_cnI","blue")'>cc_cnI</b><span style="display:none;" id="contactMatrix.md_working_7.datcc_cnI">The MATRIX_VECTOR_PRODUCT action with label <b>cc_cnI</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc_cnI</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="contactMatrix.md_working_7.datcm_cnI">cm_cnI</b>,<b name="contactMatrix.md_working_7.datones192">ones192</b>
<span style="color:blue" class="comment"># Vector with elements that are one if coordination of methylamounium with lead is &gt;11</span>
<b name="contactMatrix.md_working_7.datmt_cnI" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datmt_cnI","contactMatrix.md_working_7.datmt_cnI","blue")'>mt_cnI</b><span style="display:none;" id="contactMatrix.md_working_7.datmt_cnI">The MORE_THAN action with label <b>mt_cnI</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt_cnI</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_7.datcc_cnI">cc_cnI</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=11 NN=12 MM=24}
<br/><span style="color:blue" class="comment"># Element wise product of these three input vectors.</span>
<span style="color:blue" class="comment"># mm[i]==1 if coordination number of corrsponding methylamounium with methylamonium is &gt;5</span>
<span style="color:blue" class="comment"># and if coordination of methylamounium with Pb is &gt;7 and if coordination of methylamounium with I &gt; 11</span>
<b name="contactMatrix.md_working_7.datmm" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datmm","contactMatrix.md_working_7.datmm","blue")'>mm</b><span style="display:none;" id="contactMatrix.md_working_7.datmm">The CUSTOM action with label <b>mm</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mm</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of an arbitrary function to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_7.datmt_cncn">mt_cncn</b>,<b name="contactMatrix.md_working_7.datmt_cnpb">mt_cnpb</b>,<b name="contactMatrix.md_working_7.datmt_cnI">mt_cnI</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=x*y*z <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<br/><span style="color:blue" class="comment"># Sum of coordination numbers and thus equal to number of methylamoniums with desired coordination numbers</span>
<b name="contactMatrix.md_working_7.datff" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datff","contactMatrix.md_working_7.datff","black")'>ff</b><span style="display:none;" id="contactMatrix.md_working_7.datff">The SUM action with label <b>ff</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ff</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="contactMatrix.md_working_7.datmm">mm</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<br/><span id="contactMatrix.md_working_7.datdefrr_short"><b name="contactMatrix.md_working_7.datrr" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datrr","contactMatrix.md_working_7.datrr","black")'>rr</b><span style="display:none;" id="contactMatrix.md_working_7.datrr">The RESTRAINT action with label <b>rr</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">rr.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">rr.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_7.datdefrr");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="contactMatrix.md_working_7.datff">ff</b> <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=62 <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=10
</span><span id="contactMatrix.md_working_7.datdefrr_long" style="display:none;"><b name="contactMatrix.md_working_7.datrr" onclick='showPath("contactMatrix.md_working_7.dat","contactMatrix.md_working_7.datrr","contactMatrix.md_working_7.datrr","black")'>rr</b>: <div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("contactMatrix.md_working_7.datdefrr");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="contactMatrix.md_working_7.datff">ff</b> <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=62 <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=10  <div class="tooltip">SLOPE<div class="right"> specifies that the restraint is linear and what the values of the force constants on each of the variables are<i></i></div></div>=0.0
</span></pre>
 {% endraw %} 

In other words, we can quickly prototype a really rather complicated CV directly from the input file.  Furthermore, because this complicated CV is constructed from simpler pieces it is 
hopefully easier for other researchers to quickly understand what the CV is calculating.

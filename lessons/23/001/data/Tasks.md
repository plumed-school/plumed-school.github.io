# The task loop in detail

In some of the articles previous to this one we have discussed how we can use PLUMED to compute and print the number of distances
less than a threshold using an input similar to this one:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_Tasks.md_working_1.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="Tasks.md_working_1.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="Tasks.md_working_1.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="Tasks.md_working_1.datd1" onclick='showPath("Tasks.md_working_1.dat","Tasks.md_working_1.datd1","Tasks.md_working_1.datd1","blue")'>d1</b><span style="display:none;" id="Tasks.md_working_1.datd1">The DISTANCE action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1</td><td width="5%"><font color="blue">vector</font></td><td>the DISTANCE for each set of specified atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS1<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=1,2 <div class="tooltip">ATOMS2<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=3,4 <div class="tooltip">ATOMS3<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=5,6
<b name="Tasks.md_working_1.datd1l" onclick='showPath("Tasks.md_working_1.dat","Tasks.md_working_1.datd1l","Tasks.md_working_1.datd1l","blue")'>d1l</b><span style="display:none;" id="Tasks.md_working_1.datd1l">The LESS_THAN action with label <b>d1l</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1l</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the input is less than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">LESS_THAN<div class="right">Use a switching function to determine how many of the input variables are less than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_e_s_s__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_1.datd1">d1</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=0.1}
<b name="Tasks.md_working_1.datd1s" onclick='showPath("Tasks.md_working_1.dat","Tasks.md_working_1.datd1s","Tasks.md_working_1.datd1s","black")'>d1s</b><span style="display:none;" id="Tasks.md_working_1.datd1s">The SUM action with label <b>d1s</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1s</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_1.datd1l">d1l</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the values that you would like to print to the file<i></i></div></div>=<b name="Tasks.md_working_1.datd1s">d1s</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

In this article we are going to discuss how PLUMED does this calculation in a little more detail.  Lets therefore start by looking 
at the graph that shows how data passes through the code in this calculation:

```mermaid
flowchart TB 
MD(positions from MD)
Box("label=Box 
 PBC 
")
Box -- Box --> d1
linkStyle 0 stroke:red,color:red;
MD --> d1
linkStyle 1 stroke:violet,color:violet;
subgraph subd1 [d1]
d1(["label=d1 
 DISTANCE 
"])
d1l(["label=d1l 
 LESS_THAN 
"])
d1s(["label=d1s 
 SUM 
"])
end
d1 -- d1 --> d1l
linkStyle 2 stroke:blue,color:blue;
d1l -- d1l --> d1s
linkStyle 3 stroke:blue,color:blue;
d1s -- d1s --> 6
6("label=#64;6 
 PRINT
FILE=colvar 
")

```
{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_Tasks.md_working_2.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="Tasks.md_working_2.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="Tasks.md_working_2.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="Tasks.md_working_2.datd1" onclick='showPath("Tasks.md_working_2.dat","Tasks.md_working_2.datd1","Tasks.md_working_2.datd1","blue")'>d1</b><span style="display:none;" id="Tasks.md_working_2.datd1">The DISTANCE action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1</td><td width="5%"><font color="blue">vector</font></td><td>the DISTANCE for each set of specified atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS1<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=1,2 <div class="tooltip">ATOMS2<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=3,4 <div class="tooltip">ATOMS3<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=5,6
<b name="Tasks.md_working_2.datd1l" onclick='showPath("Tasks.md_working_2.dat","Tasks.md_working_2.datd1l","Tasks.md_working_2.datd1l","blue")'>d1l</b><span style="display:none;" id="Tasks.md_working_2.datd1l">The LESS_THAN action with label <b>d1l</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1l</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the input is less than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">LESS_THAN<div class="right">Use a switching function to determine how many of the input variables are less than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_e_s_s__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_2.datd1">d1</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=0.1}
<b name="Tasks.md_working_2.datd1s" onclick='showPath("Tasks.md_working_2.dat","Tasks.md_working_2.datd1s","Tasks.md_working_2.datd1s","black")'>d1s</b><span style="display:none;" id="Tasks.md_working_2.datd1s">The SUM action with label <b>d1s</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1s</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_2.datd1l">d1l</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the values that you would like to print to the file<i></i></div></div>=<b name="Tasks.md_working_2.datd1s">d1s</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

You can cleearly see that the actions d1, d1l and d1s are all in the same subgraph.  The calculation parts of these actions are thu all 
performed when you call the calculate method for d1.  The calculate methods for d1l and d1s do nothing.

Within d1's calculate method we call a function in ActionWithVector that is called runAllTasks, which includes the following c++ code:

```c++
#pragma omp parallel num_threads(nt)
{
  std::vector<double> omp_buffer;
  if( nt>1 ) omp_buffer.resize( bufsize, 0.0 );
  MultiValue myvals( nquants, nderivatives, nmatrices, maxcol, nbooks );
  myvals.clearAll(true);

  #pragma omp for nowait
  for(unsigned i=rank; i<nactive_tasks; i+=stride) {
    // Calculate the stuff in the loop for this action
    runTask( partialTaskList[i], myvals );

    // Now transfer the data to the actions that accumulate values from the calculated quantities
    if( nt>1 ) gatherAccumulators( partialTaskList[i], myvals, omp_buffer );
    else gatherAccumulators( partialTaskList[i], myvals, buffer );

    // Clear the value
    myvals.clearAll(true);
  }
  #pragma omp critical
  gatherThreads( nt, bufsize, omp_buffer, buffer, myvals );
}

// MPI Gather everything
if( !serial && buffer.size()>0 ) gatherProcesses( buffer );
finishComputations( buffer );
```

We can understand this code better once we recognise that d1s is calculating:

$$
s = \sigma( d_{12} ) + \sigma( d_{34} ) + \sigma( d_{56} )
$$

In this expression $d_{12}$, $d_{34}$ and $d_{56}$ are the distances between the pairs of atoms and $\sigma$ is the switching function that is used in the LESS_THAN action 
d1l. 

Each of the tasks that the loop in the c++ code runs above runs over computes one of the terms in this series.  Remember that the loop above is triggered when the calculate 
method for the action d1 is called.  Consequently, the calls to runTask are calls to the runTask method for the action d1.  The code for this method is as follows:

```c++
void ActionWithVector::runTask( const unsigned& current, MultiValue& myvals ) const {
  if( isActive() ) {
    myvals.setTaskIndex(current); myvals.vector_call=true; performTask( current, myvals );
  } 
  if( action_to_do_after ) action_to_do_after->runTask( current, myvals );
}   
``` 

This code calls the performTask method for d1 (which computes the disance). The runTask method for the action after this one in the chain, which is the runTask method for d1s.
This method transforms the distance by the switching function and then calls the runTask method for d1s, which adds the transformed distance to the scalar that we are accumulating 
here.

Notice that the derivatives of the final scalar $s$ that we are computing here with respect to each of the atomic positions $x_i$ is given by:

$$
\frac{\partial s}{\partial x_i} = \frac{\partial \sigma}{\partial d_{12}}\frac{\partial d_{12}}{\partial x_i} + \frac{\partial \sigma}{\partial d_{34}}\frac{\partial d_{34}}{\partial x_i} + \frac{\partial \sigma}{\partial d_{56}}\frac{\partial d_{56}}{\partial x_i}
$$  

If these derivatives are required (i.e. if there is a force on s) then they are also computed when we call runTask.  The information on the values and derivatives of the elements of the 
vectors d1 and d1l are passed between actions in `myvals`, which is an object of type MultiValue.  The information in myvals on each element of the vector is deleted before the start of the next iteration
through the loop when `myvals.clearAll` is called.

Information that is to be passed to Actions that are not in the chain is stored in the std::vector `buffer`.  The method `gatherAccumulators` transfers data from `myvals` to the appropriate elements of buffer.
Furthermore, if the loop is parallelised data in buffer from different threads is gathered when we call `gatherThreads` and data from different MPI processes is gathered when we call `gatherProcesses`.  The method
`finishComputations` then transfers the data from buffer to the PLMD::Value objects of the various Actions in the chain.  Notice that the methods `gatherAccumulators` and `finishComputations` have calls 
to `action_to_do_after->gatherAccumulators` and `action_to_do_after->finishComputations` at the end of them.  We thus call all these methods for all the actions in the chain when we call these actions.

## The task loop for an input with matrices

Lets now consider a second example input:

```mermaid
flowchart TB 
MD(positions from MD)
Box("label=Box 
 PBC 
")
ones(["label=ones 
 CONSTANT 
"])
Box -- Box --> c1
linkStyle 0 stroke:red,color:red;
MD --> c1
linkStyle 1 stroke:violet,color:violet;
subgraph subc1 [c1]
subgraph subc1_mat [c1]
c1(["label=c1 
 CONTACT_MATRIX 
"])
cc1(["label=cc1 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subc1_mat fill:lightblue
mt1(["label=mt1 
 MORE_THAN 
"])
subgraph subc2_mat [c2]
c2(["label=c2 
 CONTACT_MATRIX 
"])
cc2(["label=cc2 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subc2_mat fill:lightblue
mt2(["label=mt2 
 MORE_THAN 
"])
prod(["label=prod 
 CUSTOM
FUNC=x*y 
"])
s(["label=s 
 SUM 
"])
end
c1 -- c1 --> cc1
linkStyle 2 stroke:red,color:red;
ones -- ones --> cc1
linkStyle 3 stroke:blue,color:blue;
cc1 -- cc1 --> mt1
linkStyle 4 stroke:blue,color:blue;
Box -- Box --> c2
linkStyle 5 stroke:red,color:red;
MD --> c2
linkStyle 6 stroke:violet,color:violet;
c2 -- c2 --> cc2
linkStyle 7 stroke:red,color:red;
ones -- ones --> cc2
linkStyle 8 stroke:blue,color:blue;
cc2 -- cc2 --> mt2
linkStyle 9 stroke:blue,color:blue;
mt1 -- mt1 --> prod
linkStyle 10 stroke:blue,color:blue;
mt2 -- mt2 --> prod
linkStyle 11 stroke:blue,color:blue;
prod -- prod --> s
linkStyle 12 stroke:blue,color:blue;

```
{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_Tasks.md_working_3.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="Tasks.md_working_3.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="Tasks.md_working_3.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span id="Tasks.md_working_3.datones_short"><b name="Tasks.md_working_3.datones" onclick='showPath("Tasks.md_working_3.dat","Tasks.md_working_3.datones","Tasks.md_working_3.datones_shortcut","blue")'>ones</b><span style="display:none;" id="Tasks.md_working_3.datones_shortcut">The ONES action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("Tasks.md_working_3.datones");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=100
</span><span id="Tasks.md_working_3.datones_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("Tasks.md_working_3.datones")'># ones: ONES SIZE=100</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="Tasks.md_working_3.datones" onclick='showPath("Tasks.md_working_3.dat","Tasks.md_working_3.datones","Tasks.md_working_3.datones","blue")'>ones</b><span style="display:none;" id="Tasks.md_working_3.datones">The CONSTANT action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><b name="Tasks.md_working_3.datc1" onclick='showPath("Tasks.md_working_3.dat","Tasks.md_working_3.datc1","Tasks.md_working_3.datc1","red")'>c1</b><span style="display:none;" id="Tasks.md_working_3.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUPA=1-10 GROUPB=11-110 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.3 D_MAX=0.5}
<b name="Tasks.md_working_3.datcc1" onclick='showPath("Tasks.md_working_3.dat","Tasks.md_working_3.datcc1","Tasks.md_working_3.datcc1","blue")'>cc1</b><span style="display:none;" id="Tasks.md_working_3.datcc1">The MATRIX_VECTOR_PRODUCT action with label <b>cc1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc1</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="Tasks.md_working_3.datc1">c1</b>,<b name="Tasks.md_working_3.datones">ones</b>
<b name="Tasks.md_working_3.datmt1" onclick='showPath("Tasks.md_working_3.dat","Tasks.md_working_3.datmt1","Tasks.md_working_3.datmt1","blue")'>mt1</b><span style="display:none;" id="Tasks.md_working_3.datmt1">The MORE_THAN action with label <b>mt1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt1</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_3.datcc1">cc1</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=1}
<br/><b name="Tasks.md_working_3.datc2" onclick='showPath("Tasks.md_working_3.dat","Tasks.md_working_3.datc2","Tasks.md_working_3.datc2","red")'>c2</b><span style="display:none;" id="Tasks.md_working_3.datc2">The CONTACT_MATRIX action with label <b>c2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c2</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUPA=1-10 GROUPB=101-200 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.1 D_MAX=0.3}
<b name="Tasks.md_working_3.datcc2" onclick='showPath("Tasks.md_working_3.dat","Tasks.md_working_3.datcc2","Tasks.md_working_3.datcc2","blue")'>cc2</b><span style="display:none;" id="Tasks.md_working_3.datcc2">The MATRIX_VECTOR_PRODUCT action with label <b>cc2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc2</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="Tasks.md_working_3.datc2">c2</b>,<b name="Tasks.md_working_3.datones">ones</b>
<b name="Tasks.md_working_3.datmt2" onclick='showPath("Tasks.md_working_3.dat","Tasks.md_working_3.datmt2","Tasks.md_working_3.datmt2","blue")'>mt2</b><span style="display:none;" id="Tasks.md_working_3.datmt2">The MORE_THAN action with label <b>mt2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt2</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_3.datcc2">cc2</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=4}
<br/><b name="Tasks.md_working_3.datprod" onclick='showPath("Tasks.md_working_3.dat","Tasks.md_working_3.datprod","Tasks.md_working_3.datprod","blue")'>prod</b><span style="display:none;" id="Tasks.md_working_3.datprod">The CUSTOM action with label <b>prod</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">prod</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of an arbitrary function to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_3.datmt1">mt1</b>,<b name="Tasks.md_working_3.datmt2">mt2</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=x*y <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<b name="Tasks.md_working_3.dats" onclick='showPath("Tasks.md_working_3.dat","Tasks.md_working_3.dats","Tasks.md_working_3.dats","black")'>s</b><span style="display:none;" id="Tasks.md_working_3.dats">The SUM action with label <b>s</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">s</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_3.datprod">prod</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
</pre>
 {% endraw %} 

The CV here can be expressed as:

$$
s = \sum_{i=1}^{10} \sigma_{mt1}\left( \sum_{j=11}^{100} \sigma_{c1}(r_{ij}) \right)\sigma_{mt2}\left( \sum_{k=101}^{200} \sigma_{c2}(r_{ik}) \right) 
$$

where $r_{ij}$ is the distance between atoms $i$ and $j$ and $\sigma_l$ is the sigmoid function that is defined in the action with label $l$.

You can see the graph that shows how data passes through the code below:

```mermaid
flowchart TB 
MD(positions from MD)
Box("label=Box 
 PBC 
")
ones(["label=ones 
 CONSTANT 
"])
Box -- Box --> c1
linkStyle 0 stroke:red,color:red;
MD --> c1
linkStyle 1 stroke:violet,color:violet;
subgraph subc1 [c1]
subgraph subc1_mat [c1]
c1(["label=c1 
 CONTACT_MATRIX 
"])
cc1(["label=cc1 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subc1_mat fill:lightblue
mt1(["label=mt1 
 MORE_THAN 
"])
subgraph subc2_mat [c2]
c2(["label=c2 
 CONTACT_MATRIX 
"])
cc2(["label=cc2 
 MATRIX_VECTOR_PRODUCT 
"])
end
style subc2_mat fill:lightblue
mt2(["label=mt2 
 MORE_THAN 
"])
prod(["label=prod 
 CUSTOM
FUNC=x*y 
"])
s(["label=s 
 SUM 
"])
end
c1 -- c1 --> cc1
linkStyle 2 stroke:red,color:red;
ones -- ones --> cc1
linkStyle 3 stroke:blue,color:blue;
cc1 -- cc1 --> mt1
linkStyle 4 stroke:blue,color:blue;
Box -- Box --> c2
linkStyle 5 stroke:red,color:red;
MD --> c2
linkStyle 6 stroke:violet,color:violet;
c2 -- c2 --> cc2
linkStyle 7 stroke:red,color:red;
ones -- ones --> cc2
linkStyle 8 stroke:blue,color:blue;
cc2 -- cc2 --> mt2
linkStyle 9 stroke:blue,color:blue;
mt1 -- mt1 --> prod
linkStyle 10 stroke:blue,color:blue;
mt2 -- mt2 --> prod
linkStyle 11 stroke:blue,color:blue;
prod -- prod --> s
linkStyle 12 stroke:blue,color:blue;

```
{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_Tasks.md_working_4.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="Tasks.md_working_4.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="Tasks.md_working_4.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span id="Tasks.md_working_4.datones_short"><b name="Tasks.md_working_4.datones" onclick='showPath("Tasks.md_working_4.dat","Tasks.md_working_4.datones","Tasks.md_working_4.datones_shortcut","blue")'>ones</b><span style="display:none;" id="Tasks.md_working_4.datones_shortcut">The ONES action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>a vector of ones with the required number of elements</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("Tasks.md_working_4.datones");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=100
</span><span id="Tasks.md_working_4.datones_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("Tasks.md_working_4.datones")'># ones: ONES SIZE=100</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="Tasks.md_working_4.datones" onclick='showPath("Tasks.md_working_4.dat","Tasks.md_working_4.datones","Tasks.md_working_4.datones","blue")'>ones</b><span style="display:none;" id="Tasks.md_working_4.datones">The CONSTANT action with label <b>ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NOLOG<div class="right"> do not report all the read in scalars in the log<i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1
<span style="color:blue"># --- End of included input --- </span></span><b name="Tasks.md_working_4.datc1" onclick='showPath("Tasks.md_working_4.dat","Tasks.md_working_4.datc1","Tasks.md_working_4.datc1","red")'>c1</b><span style="display:none;" id="Tasks.md_working_4.datc1">The CONTACT_MATRIX action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c1</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUPA=1-10 GROUPB=11-110 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.3 D_MAX=0.5}
<b name="Tasks.md_working_4.datcc1" onclick='showPath("Tasks.md_working_4.dat","Tasks.md_working_4.datcc1","Tasks.md_working_4.datcc1","blue")'>cc1</b><span style="display:none;" id="Tasks.md_working_4.datcc1">The MATRIX_VECTOR_PRODUCT action with label <b>cc1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc1</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="Tasks.md_working_4.datc1">c1</b>,<b name="Tasks.md_working_4.datones">ones</b>
<b name="Tasks.md_working_4.datmt1" onclick='showPath("Tasks.md_working_4.dat","Tasks.md_working_4.datmt1","Tasks.md_working_4.datmt1","blue")'>mt1</b><span style="display:none;" id="Tasks.md_working_4.datmt1">The MORE_THAN action with label <b>mt1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt1</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_4.datcc1">cc1</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=1}
<br/><b name="Tasks.md_working_4.datc2" onclick='showPath("Tasks.md_working_4.dat","Tasks.md_working_4.datc2","Tasks.md_working_4.datc2","red")'>c2</b><span style="display:none;" id="Tasks.md_working_4.datc2">The CONTACT_MATRIX action with label <b>c2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">c2</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> GROUPA=1-10 GROUPB=101-200 <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=0.1 D_MAX=0.3}
<b name="Tasks.md_working_4.datcc2" onclick='showPath("Tasks.md_working_4.dat","Tasks.md_working_4.datcc2","Tasks.md_working_4.datcc2","blue")'>cc2</b><span style="display:none;" id="Tasks.md_working_4.datcc2">The MATRIX_VECTOR_PRODUCT action with label <b>cc2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cc2</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label for the matrix and the vector/scalar that are being multiplied<i></i></div></div>=<b name="Tasks.md_working_4.datc2">c2</b>,<b name="Tasks.md_working_4.datones">ones</b>
<b name="Tasks.md_working_4.datmt2" onclick='showPath("Tasks.md_working_4.dat","Tasks.md_working_4.datmt2","Tasks.md_working_4.datmt2","blue")'>mt2</b><span style="display:none;" id="Tasks.md_working_4.datmt2">The MORE_THAN action with label <b>mt2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt2</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the if the input is more than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">MORE_THAN<div class="right">Use a switching function to determine how many of the input variables are more than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_r_e__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_4.datcc2">cc2</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=4}
<br/><b name="Tasks.md_working_4.datprod" onclick='showPath("Tasks.md_working_4.dat","Tasks.md_working_4.datprod","Tasks.md_working_4.datprod","blue")'>prod</b><span style="display:none;" id="Tasks.md_working_4.datprod">The CUSTOM action with label <b>prod</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">prod</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of an arbitrary function to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_4.datmt1">mt1</b>,<b name="Tasks.md_working_4.datmt2">mt2</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=x*y <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<b name="Tasks.md_working_4.dats" onclick='showPath("Tasks.md_working_4.dat","Tasks.md_working_4.dats","Tasks.md_working_4.dats","black")'>s</b><span style="display:none;" id="Tasks.md_working_4.dats">The SUM action with label <b>s</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">s</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values input to this function<i></i></div></div>=<b name="Tasks.md_working_4.datprod">prod</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
</pre>
 {% endraw %} 

This graph tells us that the whole calculation above is done when we call the calculate method for the action with label c1.  This method calls `runAllTasks` and the 
task in the c++ loop that was shown above are the various terms in the sum over $i$ in the expression above.

The code for the `performTask` methods for the CONTACT_MATRIX actions in the above input is the one from ActionWithMatrix that looks as follows:

```c++
void ActionWithMatrix::performTask( const unsigned& task_index, MultiValue& myvals ) const {
  std::vector<unsigned> & indices( myvals.getIndices() );
  if( !doInnerLoop && actionInChain() ) {
      plumed_dbg_assert( myvals.inVectorCall() );
      runEndOfRowJobs( task_index, indices, myvals );
      return;
  }
  setupForTask( task_index, indices, myvals );

  // Now loop over the row of the matrix
  unsigned ntwo_atoms = myvals.getSplitIndex();
  for(unsigned i=0;i<ntwo_atoms;++i) {
      // This does everything in the stream that is done with single matrix elements
      runTask( getLabel(), task_index, indices[i], myvals );
      // Now clear only elements that are not accumulated over whole row
      clearMatrixElements( myvals );
  }
  // This updates the jobs that need to be completed when we get to the end of a row of the matrix 
  runEndOfRowJobs( task_index, indices, myvals );
}
```

The loop here runs over the columns of the matrix, although the method `setupForTask` uses linked lists and neighbour lists to ensure that we skip any matrix elements that we know to be zero.
Notice that when we call `runTask` within this loop this calls every method that requires the matrix elements.  In our example above, there will be a call to the runTask method in cc1 after 
each element of the c1 matrix is computed so that we can calculate the matrix vector product.

Notice, also, however, that PLUMED is clever enough to know that cc2 should not be called when we run over the elements of the c1 matrix.  The blue subgragraphs indicate the actions that PLUMED
will run over when it works through the various elements in each column of the matrix.

## Conclusion

This article is not exaustive.  A lot of the implementation detail in the code is rather complicated.  This code is necessary for ensuring that PLUMED keeps track of the non zero elements of the derivatives. 
I hope that this article at least explains how this code is supposed to work and that the interested reader can work out the remaining details by reading the code.  

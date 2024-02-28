# Backwards compatibility for MultiColvar

As discussed in [this article](MultiColvar.md), I have made substantial changes to the way MultiColvars are implemented. In previous version the PLUMED
input to calculate the number of distances are less than 0.1 nm is as follows:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_this_input_should_work.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="this_input_should_work.datd1" onclick='showPath("this_input_should_work.dat","this_input_should_work.datd1")'>d1</b>: <div class="tooltip" style="color:green">DISTANCES<div class="right">Calculate the distances between one or many pairs of atoms.  You can then calculate functions of the distribution of <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS1<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=1,2 <div class="tooltip">ATOMS2<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=3,4 <div class="tooltip">ATOMS3<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=5,6 <div class="tooltip">ATOMS4<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=7,8 <div class="tooltip">ATOMS5<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=9,10 <div class="tooltip">LESS_THAN<div class="right">calculate the number of variables less than a certain target value<i></i></div></div>={RATIONAL R_0=0.1}
<span style="display:none;" id="this_input_should_work.datd1">The DISTANCES action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1.lessthan</td><td>the number of values less than a target value</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="this_input_should_work.datd1">d1.lessthan</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

Now, however, the same operation is achieved by the following code:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_this_input_should_work.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="this_input_should_work.datd1" onclick='showPath("this_input_should_work.dat","this_input_should_work.datd1")'>d1</b>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS1<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=1,2 <div class="tooltip">ATOMS2<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=3,4 <div class="tooltip">ATOMS3<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=5,6 <div class="tooltip">ATOMS4<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=7,8 <div class="tooltip">ATOMS5<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=9,10
<span style="display:none;" id="this_input_should_work.datd1">The DISTANCE action with label <b>d1</b> calculates a scalar quantity</span><b name="this_input_should_work.datd1_lt" onclick='showPath("this_input_should_work.dat","this_input_should_work.datd1_lt")'>d1_lt</b>: <div class="tooltip" style="color:green">LESS_THAN<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ARG=<b name="this_input_should_work.datd1">d1</b> SWITCH={RATIONAL R_0=0.1}
<b name="this_input_should_work.datd1_lessthan" onclick='showPath("this_input_should_work.dat","this_input_should_work.datd1_lessthan")'>d1_lessthan</b>: <div class="tooltip" style="color:green">SUM<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ARG=d1l PERIODIC=NO
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="this_input_should_work.datd1_lessthan">d1_lessthan</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

Obviously, we do not want users to have to re-learn PLUMED because there have been changes to the code.  In other words, we want to ensure that the first
input above continues to work with the new version of the code.  

## Shortcut actions

It is straightforward to write code that allows users to use the old old PLUMED input syntax.  It is a matter of simply using shortcut actions to read 
the input for actions that are no longer implemented and convert them to the new input.  In other words, and for the example above, the command
DISTANCES is connected to a class that inherits from ActionShortcut.  In the constructor for this object the new input could be created as follows:

```c++
std::string inum, atomstr;  
for(unsigned i=1;;++i) {
    std::string atstring; parseNumbered("ATOMS",i,atstring);
    if( atstring.length()==0 ) break;
    Tools::convert( i, inum ); atomstr += " ATOMS" + inum + "=" + atstring;
}
// Create the action to compute all the distances
readInputLine( getShortcutLabel() + ": DISTANCE" + atomsstr );
// Create the LESS_THAN line
std::string lt_string; parse("LESS_THAN", lt_string );
readInputLine( getShortcutLabel() + "_lt: LESS_THAN ARG=" + getShortcutLabel() + " SWITCH={" + lt_string + "}");
// And finally the sum
readInputLine( getShortcutLabel() + "_lessthan: SUM ARG=" + getShortcutLabel() + "_lt PERIODIC=NO");
```  

This is the essense of what is done in `multicolvar/Distances.cpp` which is where the DISTANCES command is implemented within PLUMED.  The actual code 
is slightly more complicated as DISTANCES allowed for more options than simply LESS_THAN.  However, the key point I am trying to explain here is how 
we can use ActionShortcut objects to implement a single-line version of the three-line input required to calculate the number of distances that are less than 0.1 nm.

## Components of Shortcut actions

Before concluding there is one final thing I need to explain for you to fully understand how these ActionShortcut objects work. There is a wrinkle that is best 
understood by considering the following (old-style) PLUMED input again:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_this_input_should_work.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue"># This is a shortcut</span>
<b name="this_input_should_work.datd1" onclick='showPath("this_input_should_work.dat","this_input_should_work.datd1")'>d1</b>: <div class="tooltip" style="color:green">DISTANCES<div class="right">Calculate the distances between one or many pairs of atoms.  You can then calculate functions of the distribution of <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS1<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=1,2 <div class="tooltip">ATOMS2<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=3,4 <div class="tooltip">ATOMS3<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=5,6 <div class="tooltip">ATOMS4<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=7,8 <div class="tooltip">ATOMS5<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=9,10 <div class="tooltip">LESS_THAN<div class="right">calculate the number of variables less than a certain target value<i></i></div></div>={RATIONAL R_0=0.1}
<span style="color:blue"># This is not a shortcut</span>
<span style="display:none;" id="this_input_should_work.datd1">The DISTANCES action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1.lessthan</td><td>the number of values less than a target value</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="this_input_should_work.datd1">d1.lessthan</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 
 
As explained above, once the shortcuts have worked their magic PLUMED will actually read in:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_this_input_should_work.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue"># This is the expanded shortcut</span>
<b name="this_input_should_work.datd1" onclick='showPath("this_input_should_work.dat","this_input_should_work.datd1")'>d1</b>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS1<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=1,2 <div class="tooltip">ATOMS2<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=3,4 <div class="tooltip">ATOMS3<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=5,6 <div class="tooltip">ATOMS4<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=7,8 <div class="tooltip">ATOMS5<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=9,10
<span style="display:none;" id="this_input_should_work.datd1">The DISTANCE action with label <b>d1</b> calculates a scalar quantity</span><b name="this_input_should_work.datd1_lt" onclick='showPath("this_input_should_work.dat","this_input_should_work.datd1_lt")'>d1_lt</b>: <div class="tooltip" style="color:green">LESS_THAN<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ARG=<b name="this_input_should_work.datd1">d1</b> SWITCH={RATIONAL R_0=0.1}
<b name="this_input_should_work.datd1_lessthan" onclick='showPath("this_input_should_work.dat","this_input_should_work.datd1_lessthan")'>d1_lessthan</b>: <div class="tooltip" style="color:green">SUM<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ARG=d1l PERIODIC=NO
<span style="color:blue"># This is not part of the expanded shortcut</span>
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="this_input_should_work.datd1">d1.lessthan</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

The wrinkle that you need to notice here is that the quantity that we are asking PLUMED to print out `d1.lessthan` does not appear to be defined in the above input.  
The quantity that we would like to print out is called `d1_lessthan`.  Obviously, given that the input above works, there is a workaround for this problem and it is this
that still remains to be explained.  

The workaround is that you can define output components for shortcuts just as you would define output components in other ActionWithValue objects.  For our Distances action
above we can thus write a registerKeywords method as follows:

```c++
void Distances::registerKeywords(Keywords& keys) {
  ActionShortcut::registerKeywords( keys );
  keys.add("numbered","ATOMS","the pairs of atoms that you would like to calculate the angles for");
  keys.addFlag("NOPBC",false,"ignore the periodic boundary conditions when calculating distances");
  keys.add("optional","LESS_THAN","calculate the number of variables that are less than a certain target value.");
  keys.addOutputComponent("lessthan","LESS_THAN","the number of colvars that have a value less than a threshold");
```

When `ActionWithArguments` tries to interpret a Value name such as `d1.lessthan` it now does two things.

* It checks if there is an ActionWithValue object with the label `d1` that has a component called `d1.lessthan`.
* It checks if there is an ActionShortcut object with the label `d1`.  If there is such an ActionShortcut object, PLUMED checks if `lessthan` is amongst the list of registered componets for that action.  If that has indeed been registered then PLUMED interprets `d1.lessthan` as `d1_lessthan` and searches for an action with the label `d1_lessthan`

Notice that this behaviour is also triggered if you use wildcards like this:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_this_input_should_work.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="this_input_should_work.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="this_input_should_work.datd1" onclick='showPath("this_input_should_work.dat","this_input_should_work.datd1")'>d1</b>: <div class="tooltip" style="color:green">DISTANCES<div class="right">Calculate the distances between one or many pairs of atoms.  You can then calculate functions of the distribution of <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS1<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=1,2 <div class="tooltip">ATOMS2<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=3,4 <div class="tooltip">ATOMS3<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=5,6 <div class="tooltip">ATOMS4<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=7,8 <div class="tooltip">ATOMS5<div class="right">the atoms involved in each of the distances you wish to calculate<i></i></div></div>=9,10 <div class="tooltip">LOWEST<div class="right">this flag allows you to recover the lowest of these variables<i></i></div></div> <div class="tooltip">LESS_THAN<div class="right">calculate the number of variables less than a certain target value<i></i></div></div>={RATIONAL R_0=0.1}
<span style="display:none;" id="this_input_should_work.datd1">The DISTANCES action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1.lessthan</td><td>the number of values less than a target value</td></tr><tr><td width="5%">d1.lowest</td><td>the lowest of the quantities calculated by this action</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="this_input_should_work.datd1">d1</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
 {% endraw %} 

PRINT here would ouptut `d1_lessthan` and `d1_lowest` as these are the two actions that are registerd and created by the DISTANCES shortcut command.

## Conclusion

The new syntax for MultiColvar is (I think) clearer than the old one.  It also more flexible and allows one to do many more things with PLUMED.  I thus want to encourage 
users to learn it and to discard the old-style inputs in future.  To help with this aim, I have ensured that you have the option to see the full input whenever a shortcut
action appears in an example input on the tutorials page and in the nest.  You can try this functionality above.  If you hover over any of the DISTANCES commands in the example 
inputs above you will see an option to expand the shortcut.  If you click this option the full three-line input for `DISTANCES LESS_THAN` is shown.

I think that allowing users to see how code has been implemented in this way is enormously useful. Users can start understanding how the code works by interacting with the rich
set of (automatically-annotated) examples in the nest and tutorials that are likely related to the calculations they wish to perform.  They thus no longer need to battle through 
material in a manual that is full of information that is not relevant to the work they are doing. 


Specifying atoms 
----------------- 

Many of the actions in PLUMED take a list of atom positions in input. Within PLUMED 
atoms are specified using their numerical indices in the molecular dynamics input file. 

In PLUMED lists of atoms can be either provided directly inside the definition of each action, or 
predefined as a [GROUP](GROUP.md) that can be reused multiple times. Lists of atoms can be written as: 

- comma separated lists of numbers (`g1: GROUP ATOMS=10,11,15,20`) 
- numerical ranges. So `g2: GROUP ATOMS=10-20` is equivalent to `g2: GROUP ATOMS=10,11,12,13,14,15,16,17,18,19,20` 
- numerical ranges with a stride. So `g3: GROUP ATOMS=10-100:10` is equivalent to `g3: GROUP ATOMS=10,20,30,40,50,60,70,80,90,100` 
- atom ranges with a negative stride. So `g4: GROUP ATOMS=100-10:-10` is equivalent to `g4: GROUP ATOMS=100,90,80,70,60,50,40,30,20,10` 

If you want to use the atoms in a group as the input for a action you use the label of the group as shown in the following input: 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_specifying_atoms.md_working_1.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="specifying_atoms.md_working_1.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="specifying_atoms.md_working_1.datg5" onclick='showPath("specifying_atoms.md_working_1.dat","specifying_atoms.md_working_1.datg5","specifying_atoms.md_working_1.datg5","violet")'>g5</b><span style="display:none;" id="specifying_atoms.md_working_1.datg5">The GROUP action with label <b>g5</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">g5</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=1,2
<b name="specifying_atoms.md_working_1.datd1" onclick='showPath("specifying_atoms.md_working_1.dat","specifying_atoms.md_working_1.datd1","specifying_atoms.md_working_1.datd1","black")'>d1</b><span style="display:none;" id="specifying_atoms.md_working_1.datd1">The DISTANCE action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1</td><td width="5%"><font color="black">scalar</font></td><td>the DISTANCE between this pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=<b name="specifying_atoms.md_working_1.datg5">g5</b>
</pre>
 {% endraw %} 

A few other wasys of using groups in the input to actions are also available: 

- `@mdatoms` indicate all the physical atoms present in the MD engine (e.g. `DUMPATOMS ATOMS=@mdatoms`). 
- `@allatoms` indicates all atoms, including the virtual atoms that are only defined in PLUMED (e.g. `DUMPATOMS ATOMS=@allatoms`). 
- `@ndx` uses a [GROMACS index file](https://manual.gromacs.org/archive/5.0.2/online/ndx.html). `@ndx:index.ndx` picks the first group in the file. `{@ndx:{index.ndx protein}}` picks 
the group named `protein`. 

## The [MOLINFO](MOLINFO.md) command 

You can access many useful shortcuts for specifying atomic positions to PLUMED by using the MOLINFO, which takes 
a PDB structure file in input. This command allows you to access the following list of shortcuts. 

{:#browse-table .display} 
| Name | Description | 
|:---------|:---------| 
{% for item in site.data.grouplist %}| {{ item.name }} | {{ item.description }} | 
{% endfor %} 

## Virtual atoms 

Sometimes, when calculating a collective variable, you may not want to use the positions of a number of atoms directly. Instead 
you may wish to use the position of a virtual atom whose position is generated based on the positions of a collection 
of other atoms. For example you might want to use the center of mass of a group of atoms. PLUMED has a number of routines 
for calculating the positions of these virtual atoms from lists of atoms that are in the [vatom](vatom.md) module. 

To specify to an action that you want to use the position of a virtual atom to calculate an action rather than one of the atoms 
in your system you simply use the label for your virtual atom in place of the usual numerical index. Virtual 
atoms and normal atoms can be mixed together in the input to actions as shown below: 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_specifying_atoms.md_working_2.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="specifying_atoms.md_working_2.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="specifying_atoms.md_working_2.datcom1" onclick='showPath("specifying_atoms.md_working_2.dat","specifying_atoms.md_working_2.datcom1","specifying_atoms.md_working_2.datcom1","violet")'>com1</b><span style="display:none;" id="specifying_atoms.md_working_2.datcom1">The COM action with label <b>com1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">com1</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by COM action</td></tr></table></span>: <div class="tooltip" style="color:green">COM<div class="right">Calculate the center of mass for a group of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms which are involved the virtual atom's definition<i></i></div></div>=1,10 
<b name="specifying_atoms.md_working_2.datd1" onclick='showPath("specifying_atoms.md_working_2.dat","specifying_atoms.md_working_2.datd1","specifying_atoms.md_working_2.datd1","black")'>d1</b><span style="display:none;" id="specifying_atoms.md_working_2.datd1">The DISTANCE action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1</td><td width="5%"><font color="black">scalar</font></td><td>the DISTANCE between this pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=11,<b name="specifying_atoms.md_working_2.datcom1">com1</b>
</pre>
 {% endraw %} 

If you don't want to calculate CVs from the virtual atom. That is to say you just want to monitor the position of a virtual atom 
(or any set of atoms) over the course of your trajectory you can do this using DUMPATOMS. 

The list of the virtual atoms defined in PLUMED can be obtained by using the command `GROUP ATOMS=@allatoms REMOVE=@mdatoms`. 

## Broken molecules and Periodic Boundary Conditions 

PLUMED is designed so that for the majority of the CVs implemented the periodic boundary conditions are treated 
in the same manner as they would be treated in the host code. In some codes this can be problematic when the actions 
you are using involve some property of a molecule. These codes allow the atoms in the molecules to become separated by 
periodic boundaries, a fact which PLUMED could only deal with if the topology is passed from the MD code to PLUMED. Doing this 
work would involve a lot laborious programming and goes against our original aim of having a general patch that can be implemented 
in a wide variety of MD codes. Consequentially, we have implemented a more pragmatic solution to this problem - the user specifies 
in input any molecules (or parts of molecules) that must be kept in tact throughout the simulation run using the [WHOLEMOLECULES](WHOLEMOLECULES.md) command. 

The following input computes the end-to-end distance for a polymer of 100 atoms and keeps it at a value around 5. 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_specifying_atoms.md_working_3.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="specifying_atoms.md_working_3.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:green">WHOLEMOLECULES<div class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ENTITY0<div class="right">the atoms that make up a molecule that you wish to align<i></i></div></div>=1-100
<span style="display:none;" id="specifying_atoms.md_working_3.dat">The WHOLEMOLECULES action with label <b></b> calculates something</span><b name="specifying_atoms.md_working_3.date2e" onclick='showPath("specifying_atoms.md_working_3.dat","specifying_atoms.md_working_3.date2e","specifying_atoms.md_working_3.date2e","black")'>e2e</b><span style="display:none;" id="specifying_atoms.md_working_3.date2e">The DISTANCE action with label <b>e2e</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">e2e</td><td width="5%"><font color="black">scalar</font></td><td>the DISTANCE between this pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=1,100 <div class="tooltip">NOPBC<div class="right"> ignore the periodic boundary conditions when calculating distances<i></i></div></div>
<div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the values the harmonic restraint acts upon<i></i></div></div>=<b name="specifying_atoms.md_working_3.date2e">e2e</b> <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=1 <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=5
</pre>
 {% endraw %} 

Notice that NOPBC is used to in the [DISTANCE](DISTANCE.md) action so as to ensure that if the end-to-end distance is larger than half the simulation box the distance 
is compute properly. Also notice that, since many MD codes break molecules across cell boundary, it might be necessary to use the 
[WHOLEMOLECULES](WHOLEMOLECULES.md) keyword (also notice that it should be before distance). 

Notice that most expressions are invariant with respect to a change in the order of the atoms, 
but some of them depend on that order. E.g., with [WHOLEMOLECULES](WHOLEMOLECULES.md) it could be useful to 
specify atom lists in a reversed order. 

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_specifying_atoms.md_working_4.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="specifying_atoms.md_working_4.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># to see the effect, one could dump the atoms as they were before molecule reconstruction:</span>
<span style="color:blue" class="comment"># DUMPATOMS FILE=dump-broken.xyz ATOMS=1-20</span>
<div class="tooltip" style="color:green">WHOLEMOLECULES<div class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which molecules are reassembled<i></i></div></div>=1 <div class="tooltip">ENTITY0<div class="right">the atoms that make up a molecule that you wish to align<i></i></div></div>=1-20
<span style="display:none;" id="specifying_atoms.md_working_4.dat">The WHOLEMOLECULES action with label <b></b> calculates something</span><div class="tooltip" style="color:green">DUMPATOMS<div class="right">Dump selected atoms on a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_u_m_p_a_t_o_m_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file on which to output coordinates; extension is automatically detected<i></i></div></div>=dump.xyz <div class="tooltip">ATOMS<div class="right">the atom indices whose positions you would like to print out<i></i></div></div>=1-20
</pre>
 {% endraw %} 

Notice that there are other ways to manipulate the coordinates stored within PLUMED: 

- [FIT_TO_TEMPLATE](FIT_TO_TEMPLATE.md) aligns atoms to a template structure. 
- [WRAPAROUND](WRAPAROUND.md) brings a set of atom as close as possible to another set of atoms. 
- [RESET_CELL](RESET_CELL.md) rotates the periodic cell. 

<script> 
$(document).ready(function() { 
var table = $('#browse-table').DataTable({ 
"dom": '<"search"f><"top"il>rt<"bottom"Bp><"clear">', 
language: { search: '', searchPlaceholder: "Search project..." }, 
buttons: [ 
'copy', 'excel', 'pdf' 
], 
"order": [[ 0, "desc" ]] 
}); 
$('#browse-table-searchbar').keyup(function () { 
table.search( this.value ).draw(); 
}); 
hu = window.location.search.substring(1); 
searchfor = hu.split("="); 
if( searchfor[0]=="search" ) { 
table.search( searchfor[1] ).draw(); 
} 
}); 
</script> 

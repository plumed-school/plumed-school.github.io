# Action: CONTACT_MATRIX

| Description    | Usage |
|:--------:|:--------:|
| Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://plumed-school.github.io/browse.html?search=CONTACT_MATRIX)[![used in 37 eggs](https://img.shields.io/badge/nest-37-green.svg)](https://www.plumed-nest.org/browse.html?search=CONTACT_MATRIX) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| GROUPA | input | none |  |
| GROUPB | input | none |  |
| ATOMS | input | none | the atoms for which you would like to calculate the adjacency matrix |
| NL_CUTOFF | compulsory | none |  The cutoff for the neighbor list |
| NL_STRIDE | compulsory | none |  The frequency with which we are updating the atoms in the neighbor list |
| NN | compulsory | none |  The n parameter of the switching function  |
| MM | compulsory | none |  The m parameter of the switching function; 0 implies 2*NN |
| D_0 | compulsory | none |  The d_0 parameter of the switching function |
| R_0 | compulsory | none | The r_0 parameter of the switching function |
| SERIAL | optional | false |  do the calculation in serial |
| COMPONENTS | optional | false |  also calculate the components of the vector connecting the atoms in the contact matrix |
| NOPBC | optional | false |  don't use pbc |
| GROUP | optional | not used | specifies the list of atoms that should be assumed indistinguishable |
| SWITCH | optional | not used | specify the switching function to use between two sets of indistinguishable atoms |

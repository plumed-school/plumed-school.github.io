# Action: CONTACT_MATRIX

| Description    | Usage |
|:--------|:--------:|
| Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=CONTACT_MATRIX)[![used in 37 eggs](https://img.shields.io/badge/nest-37-green.svg)](https://www.plumed-nest.org/browse.html?search=CONTACT_MATRIX)|
 | **output value** | **type** |
| a matrix containing the weights for the bonds between each pair of atoms | scalar |

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| w | scalar | COMPONENTS | a matrix containing the weights for the bonds between each pair of atoms | 
| x | scalar | COMPONENTS | the projection of the bond on the x axis | 
| y | scalar | COMPONENTS | the projection of the bond on the y axis | 
| z | scalar | COMPONENTS | the projection of the bond on the z axis | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| GROUPA | atoms |  |
| GROUPB | atoms |  |
| ATOMS | atoms | the atoms for which you would like to calculate the adjacency matrix |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
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

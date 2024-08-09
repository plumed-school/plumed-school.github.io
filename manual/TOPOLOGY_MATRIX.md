# Action: TOPOLOGY_MATRIX

| Description    | Usage |
|:--------|:--------:|
| Adjacency matrix in which two atoms are adjacent if they are connected topologically | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
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
| GROUP | atoms | the atoms for which you would like to calculate the adjacency matrix |
| GROUPA | atoms |  |
| GROUPB | atoms |  |
| ATOMS | atoms | the atoms for which you would like to calculate the adjacency matrix |
| BACKGROUND_ATOMS | atoms | the list of atoms that should be considered as part of the background density |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| GROUP | input | none | the atoms for which you would like to calculate the adjacency matrix |
| GROUPA | input | none |  |
| GROUPB | input | none |  |
| ATOMS | input | none | the atoms for which you would like to calculate the adjacency matrix |
| BACKGROUND_ATOMS | input | none | the list of atoms that should be considered as part of the background density |
| NL_CUTOFF | compulsory | none |  The cutoff for the neighbor list |
| NL_STRIDE | compulsory | none |  The frequency with which we are updating the atoms in the neighbor list |
| SWITCH | compulsory | none | This keyword is used if you want to employ an alternative to the continuous swiching function defined above |
| RADIUS | compulsory | none |  |
| CYLINDER_SWITCH | compulsory | none | a switching function on ( r_ij  |
| BIN_SIZE | compulsory | none | the size to use for the bins |
| DENSITY_THRESHOLD | compulsory | none |  |
| SIGMA | compulsory | none | the width of the function to be used for kernel density estimation |
| KERNEL | compulsory | none |  the type of kernel function to be used |
| SERIAL | optional | false |  do the calculation in serial |
| COMPONENTS | optional | false |  also calculate the components of the vector connecting the atoms in the contact matrix |
| NOPBC | optional | false |  don't use pbc |

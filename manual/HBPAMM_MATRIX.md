# [Action](actions.md): HBPAMM_MATRIX

| Description    | Usage |
|:--------|:--------:|
| Adjacency matrix in which two electronegative atoms are adjacent if they are hydrogen bonded | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a matrix containing the weights for the bonds between each pair of atoms | matrix |

## Output components

This action can calculate the [values](pecifying_arguments.html) in the following table when the associated keyword is included in the input for the action. These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| w | matrix | COMPONENTS | a matrix containing the weights for the bonds between each pair of atoms | 
| x | matrix | COMPONENTS | the projection of the bond on the x axis | 
| y | matrix | COMPONENTS | the projection of the bond on the y axis | 
| z | matrix | COMPONENTS | the projection of the bond on the z axis | 


## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| GROUP | atoms | the atoms for which you would like to calculate the adjacency matrix |
| GROUPA | atoms |  |
| GROUPB | atoms |  |
| ATOMS | atoms | the atoms for which you would like to calculate the adjacency matrix |
| GROUPC | atoms |  |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| GROUP | input | none | the atoms for which you would like to calculate the adjacency matrix |
| GROUPA | input | none |  |
| GROUPB | input | none |  |
| ATOMS | input | none | the atoms for which you would like to calculate the adjacency matrix |
| GROUPC | input | none |  |
| NL_CUTOFF | compulsory | 0.0 |  The cutoff for the neighbor list |
| NL_STRIDE | compulsory | 1 |  The frequency with which we are updating the atoms in the neighbor list |
| ORDER | compulsory | dah |  the order in which the groups are specified in the input |
| CLUSTERS | compulsory | none | the name of the file that contains the definitions of all the kernels for PAMM |
| REGULARISE | compulsory | 0.001 |  don't allow the denominator to be smaller then this value |
| GAUSS_CUTOFF | compulsory | 6.25 |  the cutoff at which to stop evaluating the kernel function is set equal to sqrt(2*x)*(max(adc)+cov(adc)) |
| SERIAL | optional | false |  do the calculation in serial |
| COMPONENTS | optional | false |  also calculate the components of the vector connecting the atoms in the contact matrix |
| NOPBC | optional | false |  don't use pbc |

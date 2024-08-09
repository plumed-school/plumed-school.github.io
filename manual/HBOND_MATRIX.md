# Action: HBOND_MATRIX

| Description    | Usage |
|:--------|:--------:|
| Adjacency matrix in which two atoms are adjacent if there is a hydrogen bond between them. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
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
| HYDROGENS | atoms | The list of atoms that can form the bridge between the two interesting parts of the structure |


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
| HYDROGENS | input | none | The list of atoms that can form the bridge between the two interesting parts of the structure |
| NL_CUTOFF | compulsory | none |  The cutoff for the neighbor list |
| NL_STRIDE | compulsory | none |  The frequency with which we are updating the atoms in the neighbor list |
| SERIAL | optional | false |  do the calculation in serial |
| COMPONENTS | optional | false |  also calculate the components of the vector connecting the atoms in the contact matrix |
| NOPBC | optional | false |  don't use pbc |
| SWITCH | optional | not used | The switchingfunction that specifies how close a pair of atoms must be together for there to be a hydrogen bond between them |
| HSWITCH | optional | not used | The switchingfunction that specifies how close the hydrogen must be to the donor atom of the hydrogen bond for it to be considered a hydrogen bond |
| ASWITCH | optional | not used | A switchingfunction that is used to specify what the angle between the vector connecting the donor atom to the acceptor atom and the vector connecting the donor atom to the hydrogen must be in order for it considered to be a hydrogen bond |

# Action: DISTANCE

| Description    | Usage |
|:--------|:--------:|
| Calculate the distance between a pair of atoms. | [![used in 4 tutorials](https://img.shields.io/badge/tutorials-4-green.svg)](https://www.plumed-tutorials.org/browse.html?search=DISTANCE)[![used in 135 eggs](https://img.shields.io/badge/nest-135-green.svg)](https://www.plumed-nest.org/browse.html?search=DISTANCE)|
 | **output value** | **type** |
| the DISTANCE between this pair of atoms | scalar |

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| x | scalar | COMPONENTS | the x-component of the vector connecting the two atoms | 
| y | scalar | COMPONENTS | the y-component of the vector connecting the two atoms | 
| z | scalar | COMPONENTS | the z-component of the vector connecting the two atoms | 
| a | scalar | SCALED_COMPONENTS | the normalized projection on the first lattice vector of the vector connecting the two atoms | 
| b | scalar | SCALED_COMPONENTS | the normalized projection on the second lattice vector of the vector connecting the two atoms | 
| c | scalar | SCALED_COMPONENTS | the normalized projection on the third lattice vector of the vector connecting the two atoms | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the pair of atom that we are calculating the distance between |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the pair of atom that we are calculating the distance between |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| COMPONENTS | optional | false |  calculate the x, y and z components of the distance separately and store them as label |
| SCALED_COMPONENTS | optional | false |  calculate the a, b and c scaled components of the distance separately and store them as label |

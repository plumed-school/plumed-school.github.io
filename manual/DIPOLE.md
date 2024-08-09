# Action: DIPOLE

| Description    | Usage |
|:--------|:--------:|
| Calculate the dipole moment for a group of atoms. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the DIPOLE for these atoms | scalar |

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| x | scalar | COMPONENTS | the x-component of the dipole | 
| y | scalar | COMPONENTS | the y-component of the dipole | 
| z | scalar | COMPONENTS | the z-component of the dipole | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| GROUP | atoms | the group of atoms we are calculating the dipole moment for |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| GROUP | input | none | the group of atoms we are calculating the dipole moment for |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| COMPONENTS | optional | false |  calculate the x, y and z components of the dipole separately and store them as label |

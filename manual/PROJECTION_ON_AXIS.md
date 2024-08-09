# Action: PROJECTION_ON_AXIS

| Description    | Usage |
|:--------|:--------:|
| Calculate a position based on the projection along and extension from a defined axis. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=PROJECTION_ON_AXIS)|
 | **output value** | **type** |
| the value of the projection along the axis | scalar |

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| proj | scalar | COMPONENTS | The value of the projection along the axis | 
| ext | scalar | COMPONENTS | The value of the extension from the axis | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| AXIS_ATOMS | atoms | The atoms that define the direction of the axis of interest |
| ATOM | atoms | The atom whose position we want to project on the axis of interest |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| AXIS_ATOMS | input | none | The atoms that define the direction of the axis of interest |
| ATOM | input | none | The atom whose position we want to project on the axis of interest |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |

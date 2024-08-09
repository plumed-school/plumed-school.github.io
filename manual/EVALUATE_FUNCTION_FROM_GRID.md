# Action: EVALUATE_FUNCTION_FROM_GRID

| Description    | Usage |
|:--------|:--------:|
| Calculate the function stored on the input grid at an arbitrary point | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| interpolation of the input grid to get the value of the function at the input arguments | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the arguments that you would like to use when evaluating the function |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the arguments that you would like to use when evaluating the function |
| GRID | compulsory | none | the name of the grid that we are using to evaluate the function |
| INTERPOLATION_TYPE | compulsory | none |  the method to use for interpolation |
| ZERO_OUTSIDE_GRID_RANGE | optional | false |  if we are asked to evaluate the function for a number that is outside the range of the grid set it to zero |

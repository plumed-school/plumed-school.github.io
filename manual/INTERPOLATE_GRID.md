# Action: INTERPOLATE_GRID

| Description    | Usage |
|:--------|:--------:|
| Interpolate a smooth function stored on a grid onto a grid with a smaller grid spacing. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=INTERPOLATE_GRID)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| interpolation of the input grid to get the value of the function at the input arguments | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| INTERPOLATION_TYPE | compulsory | none |  the method to use for interpolation |
| SERIAL | optional | false |  do the calculation in serial |
| GRID_BIN | optional | not used | the number of bins for the grid |
| GRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with GRID_BIN) |
| MIDPOINTS | optional | false |  interpolate the values of the function at the midpoints of the grid coordinates of the input grid |
| ZERO_OUTSIDE_GRID_RANGE | optional | false |  if we are asked to evaluate the function for a number that is outside the range of the grid set it to zero |

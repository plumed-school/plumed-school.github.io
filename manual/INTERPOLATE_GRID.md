# [Action](actions.md): INTERPOLATE_GRID

| Description    | Usage |
|:--------|:--------:|
| Interpolate a smooth function stored on a grid onto a grid with a smaller grid spacing. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=INTERPOLATE_GRID)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the function evaluated onto the interpolated grid | grid |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | grid | the label for function on the grid that you would like to interpolate |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label for function on the grid that you would like to interpolate |
| INTERPOLATION_TYPE | compulsory | spline |  the method to use for interpolation |
| SERIAL | optional | false |  do the calculation in serial |
| GRID_BIN | optional | not used | the number of bins for the grid |
| GRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with GRID_BIN) |
| MIDPOINTS | optional | false |  interpolate the values of the function at the midpoints of the grid coordinates of the input grid |
| ZERO_OUTSIDE_GRID_RANGE | optional | false |  if we are asked to evaluate the function for a number that is outside the range of the grid set it to zero |

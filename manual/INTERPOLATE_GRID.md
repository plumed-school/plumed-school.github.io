# Action: INTERPOLATE_GRID

| Description    | Usage |
|:--------:|:--------:|
| Interpolate a smooth function stored on a grid onto a grid with a smaller grid spacing. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://plumed-school.github.io/browse.html?search=INTERPOLATE_GRID)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| INTERPOLATION_TYPE | compulsory | none |  the method to use for interpolation |
| SERIAL | optional | false |  do the calculation in serial |
| GRID_BIN | optional | not used | the number of bins for the grid |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |
| GRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with GRID_BIN) |
| MIDPOINTS | optional | false |  interpolate the values of the function at the midpoints of the grid coordinates of the input grid |
| ZERO_OUTSIDE_GRID_RANGE | optional | false |  if we are asked to evaluate the function for a number that is outside the range of the grid set it to zero |

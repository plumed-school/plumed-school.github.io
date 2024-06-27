# Action: FIND_CONTOUR

| Description    | Usage |
|:--------:|:--------:|
| Find an isocontour in a smooth function. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| CONTOUR | compulsory | none | the value we would like to draw the contour at in the space |
| INTERPOLATION_TYPE | compulsory | none |  the method to use for interpolation |
| BUFFER | compulsory | none |  number of buffer grid points around location where grid was found on last step |
| SERIAL | optional | false |  do the calculation in serial |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |
| ZERO_OUTSIDE_GRID_RANGE | optional | false |  if we are asked to evaluate the function for a number that is outside the range of the grid set it to zero |

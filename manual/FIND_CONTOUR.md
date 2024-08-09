# Action: FIND_CONTOUR

| Description    | Usage |
|:--------|:--------:|
| Find an isocontour in a smooth function. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| interpolation of the input grid to get the value of the function at the input arguments | scalar |

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| .#!custom | scalar | the names of the output components for this action depend on the actions input file see the example inputs below for details | 


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
| CONTOUR | compulsory | none | the value we would like to draw the contour at in the space |
| INTERPOLATION_TYPE | compulsory | none |  the method to use for interpolation |
| BUFFER | compulsory | none |  number of buffer grid points around location where grid was found on last step |
| SERIAL | optional | false |  do the calculation in serial |
| ZERO_OUTSIDE_GRID_RANGE | optional | false |  if we are asked to evaluate the function for a number that is outside the range of the grid set it to zero |

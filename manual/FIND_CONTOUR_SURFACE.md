# Action: FIND_CONTOUR_SURFACE

| Description    | Usage |
|:--------|:--------:|
| Find an isocontour by searching along either the x, y or z direction. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=FIND_CONTOUR_SURFACE)|
 | **output value** | **type** |
| a grid containing the location of the points in the Willard-Chandler surface along the chosen direction | scalar |

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
| SEARCHDIR | compulsory | none | In which directions do you wish to search for the contour |
| SERIAL | optional | false |  do the calculation in serial |
| ZERO_OUTSIDE_GRID_RANGE | optional | false |  if we are asked to evaluate the function for a number that is outside the range of the grid set it to zero |

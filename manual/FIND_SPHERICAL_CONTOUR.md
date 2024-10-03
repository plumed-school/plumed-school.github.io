# [Action](actions.md): FIND_SPHERICAL_CONTOUR

| Description    | Usage |
|:--------|:--------:|
| Find an isocontour in a three dimensional grid by searching over a Fibonacci sphere. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a grid on a Fibonacci sphere that describes the radial distance from the origin for the points on the Willard-Chandler surface | grid |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | grid | the labels of the grid in which the contour will be found |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the grid in which the contour will be found |
| CONTOUR | compulsory | none | the value we would like to draw the contour at in the space |
| INTERPOLATION_TYPE | compulsory | spline |  the method to use for interpolation |
| NPOINTS | compulsory | none | the number of points for which we are looking for the contour |
| INNER_RADIUS | compulsory | none | the minimum radius on which to look for the contour |
| OUTER_RADIUS | compulsory | none | the outer radius on which to look for the contour |
| NBINS | compulsory | 1 |  the number of discrete sections in which to divide the distance between the inner and outer radius when searching for a contour |
| SERIAL | optional | false |  do the calculation in serial |
| ZERO_OUTSIDE_GRID_RANGE | optional | false |  if we are asked to evaluate the function for a number that is outside the range of the grid set it to zero |

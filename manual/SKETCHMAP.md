# Action: SKETCHMAP

| Description    | Usage |
|:--------|:--------:|
| Construct a sketch map projection of the input data | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=SKETCHMAP)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=SKETCHMAP)|
 | **output value** | **type** |
| the sketch-map projection of the input points | scalar |

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| osample | scalar | PROJECT_ALL | the out-of-sample projections | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the matrix of high dimensional coordinates that you want to project in the low dimensional space |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the matrix of high dimensional coordinates that you want to project in the low dimensional space |
| NLOW_DIM | compulsory | none | number of low-dimensional coordinates required |
| HIGH_DIM_FUNCTION | compulsory | none | the parameters of the switching function in the high dimensional space |
| LOW_DIM_FUNCTION | compulsory | none | the parameters of the switching function in the low dimensional space |
| CGTOL | compulsory | none |  The tolerance for the conjugate gradient minimization that finds the projection of the landmarks |
| MAXITER | compulsory | none |  maximum number of optimization cycles for optimisation algorithms |
| NCYCLES | compulsory | none |  The number of cycles of pointwise global optimisation that are required |
| BUFFER | compulsory | none |  grid extent for search is (max projection - minimum projection) multiplied by this value |
| CGRID_SIZE | compulsory | none |  number of points to use in each grid direction |
| FGRID_SIZE | compulsory | none |  interpolate the grid onto this number of points -- only works in 2D |
| OS_CGTOL | compulsory | none |  The tolerance for the conjugate gradient minimization that finds the out of sample projections |
| SMACTOL | compulsory | none |  the tolerance for the smacof algorithm |
| SMACREG | compulsory | none |  this is used to ensure that we don't divide by zero when updating weights for SMACOF algorithm |
| WEIGHTS | optional | not used | a vector containing the weights of the points |
| PROJECT_ALL | optional | false |  if the input are landmark coordinates then project the out of sample configurations |
| USE_SMACOF | optional | false |  find the projection in the low dimensional space using the SMACOF algorithm |

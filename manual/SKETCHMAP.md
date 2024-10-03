# [Shortcut](shortcuts.md): SKETCHMAP

| Description    | Usage |
|:--------|:--------:|
| Construct a sketch map projection of the input data | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=SKETCHMAP)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=SKETCHMAP)|
 | **output value** | **type** |
| the sketch-map projection of the input points | matrix |

## Output components

This action can calculate the [values](pecifying_arguments.html) in the following table when the associated keyword is included in the input for the action. These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| osample | matrix | PROJECT_ALL | the out-of-sample projections | 


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| NLOW_DIM | compulsory | none | number of low-dimensional coordinates required |
| ARG | compulsory | none | the matrix of high dimensional coordinates that you want to project in the low dimensional space |
| HIGH_DIM_FUNCTION | compulsory | none | the parameters of the switching function in the high dimensional space |
| LOW_DIM_FUNCTION | compulsory | none | the parameters of the switching function in the low dimensional space |
| CGTOL | compulsory | 1E-6 |  The tolerance for the conjugate gradient minimization that finds the projection of the landmarks |
| MAXITER | compulsory | 1000 |  maximum number of optimization cycles for optimisation algorithms |
| NCYCLES | compulsory | 0 |  The number of cycles of pointwise global optimisation that are required |
| BUFFER | compulsory | 1.1 |  grid extent for search is (max projection - minimum projection) multiplied by this value |
| CGRID_SIZE | compulsory | 10 |  number of points to use in each grid direction |
| FGRID_SIZE | compulsory | 0 |  interpolate the grid onto this number of points -- only works in 2D |
| OS_CGTOL | compulsory | 1E-6 |  The tolerance for the conjugate gradient minimization that finds the out of sample projections |
| SMACTOL | compulsory | 1E-4 |  the tolerance for the smacof algorithm |
| SMACREG | compulsory | 0.001 |  this is used to ensure that we don't divide by zero when updating weights for SMACOF algorithm |
| WEIGHTS | optional | not used | a vector containing the weights of the points |
| PROJECT_ALL | optional | false |  if the input are landmark coordinates then project the out of sample configurations |
| USE_SMACOF | optional | false |  find the projection in the low dimensional space using the SMACOF algorithm |

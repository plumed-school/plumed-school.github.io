# Action: SPHERICAL_KDE

| Description    | Usage |
|:--------|:--------:|
| Create a histogram from the input scalar/vector/matrix using SPHERICAL_KDE | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a function on a grid that was obtained by doing a Kernel Density Estimation using the input arguments | scalar |

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
| GRID_MIN | compulsory | none |  the lower bounds for the grid |
| GRID_MAX | compulsory | none |  the upper bounds for the grid |
| METRIC | compulsory | none | the inverse covariance to use for the kernels that are added to the grid |
| CUTOFF | compulsory | none |  the cutoff at which to stop evaluating the kernel functions is set equal to sqrt(2*x)*bandwidth in each direction where x is this number |
| KERNEL | compulsory | none |  the kernel function you are using |
| CONCENTRATION | compulsory | none | the concentration parameter for Von Mises-Fisher distributions (only required for SPHERICAL_KDE) |
| SERIAL | optional | false |  do the calculation in serial |
| HEIGHTS | optional | not used | this keyword takes the label of an action that calculates a vector of values |
| VOLUMES | optional | not used | this keyword take the label of an action that calculates a vector of values |
| BANDWIDTH | optional | not used | the bandwidths for kernel density esimtation |
| GRID_BIN | optional | not used | the number of bins for the grid |
| IGNORE_IF_OUT_OF_RANGE | optional | false |  if a kernel is outside of the range of the grid it is safe to ignore |
| GRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with GRID_BIN) |

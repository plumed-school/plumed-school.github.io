# Action: HISTOGRAM

| Description    | Usage |
|:--------|:--------:|
| Accumulate the average probability density along a few CVs from a trajectory. | [![used in 6 tutorials](https://img.shields.io/badge/tutorials-6-green.svg)](https://www.plumed-tutorials.org/browse.html?search=HISTOGRAM)[![used in 30 eggs](https://img.shields.io/badge/nest-30-green.svg)](https://www.plumed-nest.org/browse.html?search=HISTOGRAM)|
 | **output value** | **type** |
| the estimate of the histogram as a function of the argument that was obtained | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the quantity that is being averaged |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the quantity that is being averaged |
| NORMALIZATION | compulsory | none |  This controls how the data is normalized it can be set equal to true, false or ndata |
| GRID_MIN | compulsory | none |  the lower bounds for the grid |
| GRID_MAX | compulsory | none |  the upper bounds for the grid |
| KERNEL | compulsory | none |  the kernel function you are using |
| STRIDE | compulsory | none |  the frequency with which to store data for averaging |
| CLEAR | compulsory | none |  the frequency with whihc to clear the data that is being averaged |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |
| DATA | optional | not used | an alternative to the ARG keyword |
| BANDWIDTH | optional | not used | the bandwidths for kernel density esimtation |
| GRID_BIN | optional | not used | the number of bins for the grid |
| GRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with GRID_BIN) |
| LOGWEIGHTS | optional | not used | the logarithm of the quantity to use as the weights when calculating averages |

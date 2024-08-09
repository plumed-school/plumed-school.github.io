# Action: ARRANGE_POINTS

| Description    | Usage |
|:--------|:--------:|
| Arrange points in a low dimensional space so that the (transformed) distances between points in the low dimensional space match the dissimilarities provided in an input matrix. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

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
| MINTYPE | compulsory | none |  the method to use for the minimisation |
| MAXITER | compulsory | none |  maximum number of optimization cycles for optimisation algorithms |
| CGTOL | compulsory | none |  the tolerance for the conjugate gradient minimization |
| NCYCLES | compulsory | none |  the number of cycles of global optimization to attempt |
| BUFFER | compulsory | none |  grid extent for search is (max projection - minimum projection) multiplied by this value |
| CGRID_SIZE | compulsory | none |  number of points to use in each grid direction |
| FGRID_SIZE | compulsory | none |  interpolate the grid onto this number of points -- only works in 2D |
| SMACTOL | compulsory | none |  the tolerance for the smacof algorithm |
| SMACREG | compulsory | none |  this is used to ensure that we don't divide by zero when updating weights for SMACOF algorithm |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| TARGET | optional | not used | the matrix of target quantities that you would like to match |
| FUNC | optional | not used | a function that is applied on the distances between the points in the low dimensional space |
| WEIGHTS | optional | not used | the matrix with the weights of the target quantities |

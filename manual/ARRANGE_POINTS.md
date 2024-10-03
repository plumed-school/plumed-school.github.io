# [Action](actions.md): ARRANGE_POINTS

| Description    | Usage |
|:--------|:--------:|
| Arrange points in a low dimensional space so that the (transformed) distances between points in the low dimensional space match the dissimilarities provided in an input matrix. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | vector | the initial positions for the projections |
| TARGET | matrix | the matrix of target quantities that you would like to match |
| WEIGHTS | matrix | the matrix with the weights of the target quantities |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the initial positions for the projections |
| TARGET | input | none | the matrix of target quantities that you would like to match |
| WEIGHTS | input | none | the matrix with the weights of the target quantities |
| MINTYPE | compulsory | conjgrad |  the method to use for the minimisation |
| MAXITER | compulsory | 1000 |  maximum number of optimization cycles for optimisation algorithms |
| CGTOL | compulsory | 1E-6 |  the tolerance for the conjugate gradient minimization |
| NCYCLES | compulsory | 5 |  the number of cycles of global optimization to attempt |
| BUFFER | compulsory | 1.1 |  grid extent for search is (max projection - minimum projection) multiplied by this value |
| CGRID_SIZE | compulsory | 10 |  number of points to use in each grid direction |
| FGRID_SIZE | compulsory | 0 |  interpolate the grid onto this number of points -- only works in 2D |
| SMACTOL | compulsory | 1E-4 |  the tolerance for the smacof algorithm |
| SMACREG | compulsory | 0.001 |  this is used to ensure that we don't divide by zero when updating weights for SMACOF algorithm |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| FUNC | optional | not used | a function that is applied on the distances between the points in the low dimensional space |

# [Action](actions.md): PROJECT_POINTS

| Description    | Usage |
|:--------|:--------:|
| Find the projection of a point in a low dimensional space by matching the (transformed) distance between it and a series of reference configurations that were input | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=PROJECT_POINTS)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | vector | the projections of the landmark points |
| TARGET | vector/matrix | the matrix of target quantities that you would like to match |
| WEIGHTS | vector | the matrix with the weights of the target quantities |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the projections of the landmark points |
| TARGET | input | none | the matrix of target quantities that you would like to match |
| WEIGHTS | input | none | the matrix with the weights of the target quantities |
| CGTOL | compulsory | 1E-6 |  the tolerance for the conjugate gradient minimization |
| SERIAL | optional | false |  do the calculation in serial |
| FUNC | optional | not used | a function that is applied on the distances between the points in the low dimensional space |

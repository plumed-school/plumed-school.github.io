# Action: PROJECT_POINTS

| Description    | Usage |
|:--------|:--------:|
| Find the projection of a point in a low dimensional space by matching the (transformed) distance between it and a series of reference configurations that were input | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=PROJECT_POINTS)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

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
| CGTOL | compulsory | none |  the tolerance for the conjugate gradient minimization |
| SERIAL | optional | false |  do the calculation in serial |
| TARGET | optional | not used | the matrix of target quantities that you would like to match |
| FUNC | optional | not used | a function that is applied on the distances between the points in the low dimensional space |
| WEIGHTS | optional | not used | the matrix with the weights of the target quantities |

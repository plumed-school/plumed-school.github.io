# Action: COVARIANCE_MATRIX

| Description    | Usage |
|:--------|:--------:|
| Calculate a covariance matix | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the covariance matrix | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the vectors of data from which we are calculating the covariance |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the vectors of data from which we are calculating the covariance |
| WEIGHTS | compulsory | none | this keyword takes the label of an action that calculates a vector of values |
| UNORMALIZED | optional | false |  do not divide by the sum of the weights |

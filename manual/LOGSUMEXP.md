# Action: LOGSUMEXP

| Description    | Usage |
|:--------|:--------:|
| This action takes the exponential of a vector of logarithms and divides each element of the vector by the sum of the exponentials. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the logarithms of the input weights logweights that are computed with the log-sum weights formula | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the vector of logweights that you would like to normalise using the logsumexp trick |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the vector of logweights that you would like to normalise using the logsumexp trick |

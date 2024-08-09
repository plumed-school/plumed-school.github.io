# Action: AVERAGE

| Description    | Usage |
|:--------|:--------:|
| Calculate the ensemble average of a collective variable | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=AVERAGE)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=AVERAGE)|
 | **output value** | **type** |
| the value of the average | scalar |

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
| STRIDE | compulsory | none |  the frequency with which to store data for averaging |
| CLEAR | compulsory | none |  the frequency with whihc to clear the data that is being averaged |
| LOGWEIGHTS | optional | not used | the logarithm of the quantity to use as the weights when calculating averages |
| NORMALIZATION | optional | not used | keyword for old version of the code that is there to maintain back compatibility only |

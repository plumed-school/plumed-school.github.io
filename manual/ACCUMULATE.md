# Action: ACCUMULATE

| Description    | Usage |
|:--------|:--------:|
| Sum the elements of this value over the course of the trajectory | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=ACCUMULATE)[![used in 25 eggs](https://img.shields.io/badge/nest-25-green.svg)](https://www.plumed-nest.org/browse.html?search=ACCUMULATE)|
 | **output value** | **type** |
| a sum calculated from the time series of the input quantity | scalar |

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
| STRIDE | compulsory | none |  the frequency with which the data should be collected and added to the quantity being averaged |
| CLEAR | compulsory | none |  the frequency with which to clear all the accumulated data |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

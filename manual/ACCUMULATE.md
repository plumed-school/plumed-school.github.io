# [Action](actions.md): ACCUMULATE

| Description    | Usage |
|:--------|:--------:|
| Sum the elements of this value over the course of the trajectory | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=ACCUMULATE)[![used in 24 eggs](https://img.shields.io/badge/nest-24-green.svg)](https://www.plumed-nest.org/browse.html?search=ACCUMULATE)|
 | **output value** | **type** |
| a sum calculated from the time series of the input quantity | scalar/grid |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/grid | the label of the argument that is being added to on each timestep |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label of the argument that is being added to on each timestep |
| STRIDE | compulsory | 1 |  the frequency with which the data should be collected and added to the quantity being averaged |
| CLEAR | compulsory | 0 |  the frequency with which to clear all the accumulated data |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

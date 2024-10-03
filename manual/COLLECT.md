# [Action](actions.md): COLLECT

| Description    | Usage |
|:--------|:--------:|
| Collect data from the trajectory for later analysis | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the time series for the input quantity | vector/matrix |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector/matrix | the label of the value whose time series is being stored for later analysis |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label of the value whose time series is being stored for later analysis |
| STRIDE | compulsory | 1 |  the frequency with which the data should be collected and added to the quantity being averaged |
| CLEAR | compulsory | 0 |  the frequency with which to clear all the accumulated data |
| TYPE | compulsory | auto |  required if you are collecting an object with rank>0 |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

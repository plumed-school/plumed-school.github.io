# [Action](actions.md): SELECT

| Description    | Usage |
|:--------|:--------:|
| Selects an argument based on the value of a SELECTOR. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the value of the selected argument | scalar |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of the values from which the function is calculated |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the values from which the function is calculated |
| SELECTOR | compulsory | none | name of the variable used to select |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |

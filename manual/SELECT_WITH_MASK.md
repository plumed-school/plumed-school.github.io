# Action: SELECT_WITH_MASK

| Description    | Usage |
|:--------|:--------:|
| Use a mask to select elements of an array | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a vector/matrix of values that is obtained using a mask to select elements of interest | scalar |

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
| MASK | compulsory | none | an array with ones in the components that you want to discard |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ROW_MASK | optional | not used | an array with ones in the rows of the matrix that you want to discard |
| COLUMN_MASK | optional | not used | an array with ones in the columns of the matrix that you want to discard |

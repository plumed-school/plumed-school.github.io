# [Action](actions.md): SELECT_WITH_MASK

| Description    | Usage |
|:--------|:--------:|
| Use a mask to select elements of an array | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a vector/matrix of values that is obtained using a mask to select elements of interest | vector/matrix |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector/matrix | the label for the value upon which you are going to apply the mask |
| ROW_MASK | vector | an array with ones in the rows of the matrix that you want to discard |
| COLUMN_MASK | vector | an array with ones in the columns of the matrix that you want to discard |
| MASK | vector/matrix | an array with ones in the components that you want to discard |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label for the value upon which you are going to apply the mask |
| ROW_MASK | input | none | an array with ones in the rows of the matrix that you want to discard |
| COLUMN_MASK | input | none | an array with ones in the columns of the matrix that you want to discard |
| MASK | input | none | an array with ones in the components that you want to discard |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |

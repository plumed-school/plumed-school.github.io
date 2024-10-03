# [Action](actions.md): MATRIX_PRODUCT

| Description    | Usage |
|:--------|:--------:|
| Calculate the product of two matrices | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=MATRIX_PRODUCT)[![used in 3 eggs](https://img.shields.io/badge/nest-3-green.svg)](https://www.plumed-nest.org/browse.html?search=MATRIX_PRODUCT)|
 | **output value** | **type** |
| the product of the two input matrices | matrix |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | matrix | the label of the two matrices from which the product is calculated |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label of the two matrices from which the product is calculated |
| SERIAL | optional | false |  do the calculation in serial |
| SQUARED | optional | false |  calculate the squares of the dissimilarities (this option cannot be used with MATRIX_PRODUCT) |

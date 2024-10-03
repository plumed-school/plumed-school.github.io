# [Action](actions.md): CONCATENATE

| Description    | Usage |
|:--------|:--------:|
| Join vectors or matrices together | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=CONCATENATE)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=CONCATENATE)|
 | **output value** | **type** |
| the concatenated vector/matrix that was constructed from the input values | vector/matrix |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector | the values that should be concatenated together to form the output vector |
| MATRIX | scalar/matrix | specify the matrices that you wish to join together into a single matrix |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the values that should be concatenated together to form the output vector |
| MATRIX | input | none | specify the matrices that you wish to join together into a single matrix |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |

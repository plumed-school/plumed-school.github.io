# [Action](actions.md): VSTACK

| Description    | Usage |
|:--------|:--------:|
| Create a matrix by stacking vectors together | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=VSTACK)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=VSTACK)|
 | **output value** | **type** |
| a matrix that contains the input vectors in its columns | matrix |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector | the values that you would like to stack together to construct the output matrix |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the values that you would like to stack together to construct the output matrix |
| SERIAL | optional | false |  do the calculation in serial |

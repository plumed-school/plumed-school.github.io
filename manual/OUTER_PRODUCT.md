# Action: OUTER_PRODUCT

| Description    | Usage |
|:--------|:--------:|
| Calculate the outer product matrix of two vectors | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=OUTER_PRODUCT)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=OUTER_PRODUCT)|
 | **output value** | **type** |
| a matrix containing the outer product of the two input vectors that was obtained using the function that was input | scalar |

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
| FUNC | compulsory | none |  the function of the input vectors that should be put in the elements of the outer product |
| SERIAL | optional | false |  do the calculation in serial |
| ELEMENTS_ON_DIAGONAL_ARE_ZERO | optional | false |  set all diagonal elements to zero |

# Action: VORONOI

| Description    | Usage |
|:--------|:--------:|
| Do a voronoi analysis | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=VORONOI)|
 | **output value** | **type** |
| a matrix in which element ij is equal to one if the ij component of the input matrix is lower than all the ik elements of the matrix where k is not j and zero otherwise | scalar |

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
| SERIAL | optional | false |  do the calculation in serial |

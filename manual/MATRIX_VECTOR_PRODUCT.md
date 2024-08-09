# Action: MATRIX_VECTOR_PRODUCT

| Description    | Usage |
|:--------|:--------:|
| Calculate the product of the matrix and the vector | [![used in 3 tutorials](https://img.shields.io/badge/tutorials-3-green.svg)](https://www.plumed-tutorials.org/browse.html?search=MATRIX_VECTOR_PRODUCT)[![used in 39 eggs](https://img.shields.io/badge/nest-39-green.svg)](https://www.plumed-nest.org/browse.html?search=MATRIX_VECTOR_PRODUCT)|
 | **output value** | **type** |
| the vector that is obtained by taking the product between the matrix and the vector that were input | scalar |

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| .#!custom | scalar | the names of the output components for this action depend on the actions input file see the example inputs below for details | 


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

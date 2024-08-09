# Action: NEIGHBORS

| Description    | Usage |
|:--------|:--------:|
| Build a matrix with ones in for the N nearest neighbours of an atom | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a matrix in which the ij element is one if the ij-element of the input matrix is one of the NLOWEST/NHIGHEST elements on that row of the input matrix and zero otherwise | scalar |

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
| NLOWEST | compulsory | none |  in each row of the output matrix set the elements that correspond to the n lowest elements in each row of the input matrix equal to one |
| NHIGHEST | compulsory | none |  in each row of the output matrix set the elements that correspond to the n highest elements in each row of the input matrix equal to one |
| SERIAL | optional | false |  do the calculation in serial |

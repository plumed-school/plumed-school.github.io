# Action: TORSIONS_MATRIX

| Description    | Usage |
|:--------|:--------:|
| Calculate the matrix of torsions between two vectors of molecules | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the matrix of torsions between the two vectors of input directors | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |
| POSITIONS1 | atoms | the positions to use for the molecules specified using the first argument |
| POSITIONS2 | atoms | the positions to use for the molecules specified using the second argument |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| POSITIONS1 | input | none | the positions to use for the molecules specified using the first argument |
| POSITIONS2 | input | none | the positions to use for the molecules specified using the second argument |
| SERIAL | optional | false |  do the calculation in serial |

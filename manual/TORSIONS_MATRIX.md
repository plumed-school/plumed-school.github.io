# [Action](actions.md): TORSIONS_MATRIX

| Description    | Usage |
|:--------|:--------:|
| Calculate the matrix of torsions between two vectors of molecules | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the matrix of torsions between the two vectors of input directors | matrix |

## Input

The [arguments](specifying_arguments.html) and [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | matrix | an Nx3 and a 3xN matrix that contain the bond vectors that you would like to determine the torsion angles between |
| POSITIONS1 | atoms | the positions to use for the molecules specified using the first argument |
| POSITIONS2 | atoms | the positions to use for the molecules specified using the second argument |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | an Nx3 and a 3xN matrix that contain the bond vectors that you would like to determine the torsion angles between |
| POSITIONS1 | input | none | the positions to use for the molecules specified using the first argument |
| POSITIONS2 | input | none | the positions to use for the molecules specified using the second argument |
| SERIAL | optional | false |  do the calculation in serial |

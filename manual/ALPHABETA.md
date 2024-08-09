# Action: ALPHABETA

| Description    | Usage |
|:--------|:--------:|
| Calculate the alpha beta CV | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 18 eggs](https://img.shields.io/badge/nest-18-green.svg)](https://www.plumed-nest.org/browse.html?search=ALPHABETA)|
 | **output value** | **type** |
| the alpha beta CV | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the atoms involved for each of the torsions you wish to calculate |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the atoms involved for each of the torsions you wish to calculate |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| REFERENCE | optional | not used | the reference values for each of the torsional angles |
| COEFFICIENT | optional | not used | the coefficient for each of the torsional angles |

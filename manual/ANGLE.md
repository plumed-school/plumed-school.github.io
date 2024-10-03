# [Action](actions.md): ANGLE

| Description    | Usage |
|:--------|:--------:|
| Calculate an angle. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=ANGLE)[![used in 14 eggs](https://img.shields.io/badge/nest-14-green.svg)](https://www.plumed-nest.org/browse.html?search=ANGLE)|
 | **output value** | **type** |
| the ANGLE involving these atoms | scalar/vector |

## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the list of atoms involved in this collective variable (either 3 or 4 atoms) |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the list of atoms involved in this collective variable (either 3 or 4 atoms) |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |

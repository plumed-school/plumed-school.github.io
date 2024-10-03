# [Action](actions.md): CONSTANT

| Description    | Usage |
|:--------|:--------:|
| Create a constant value that can be passed to actions | [![used in 3 tutorials](https://img.shields.io/badge/tutorials-3-green.svg)](https://www.plumed-tutorials.org/browse.html?search=CONSTANT)[![used in 33 eggs](https://img.shields.io/badge/nest-33-green.svg)](https://www.plumed-nest.org/browse.html?search=CONSTANT)|
 | **output value** | **type** |
| the constant value that was read from the plumed input | scalar/vector/matrix |

## Output components

This action can calculate the [values](pecifying_arguments.html) in the following table when the associated keyword is included in the input for the action. These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| v | scalar | SCALARS | the # value | 


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| NROWS | compulsory | 0 |  the number of rows in your input matrix |
| NCOLS | compulsory | 0 |  the number of columns in your matrix |
| FILE | optional | not used | an input file containing the matrix |
| VALUE | optional | not used | the single number that you would like to store |
| VALUES | optional | not used | the numbers that are in your constant value |
| SCALARS | optional | false |  treat the input list of numbers as a set of scalars |
| NOLOG | optional | false |  do not report all the read in scalars in the log |

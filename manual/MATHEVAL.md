# [Shortcut](shortcuts.md): MATHEVAL

| Description    | Usage |
|:--------|:--------:|
| An alias to the CUSTOM function that can also be used to calaculate combinations of variables using a custom expression. | [![used in 5 tutorials](https://img.shields.io/badge/tutorials-5-green.svg)](https://www.plumed-tutorials.org/browse.html?search=MATHEVAL)[![used in 57 eggs](https://img.shields.io/badge/nest-57-green.svg)](https://www.plumed-nest.org/browse.html?search=MATHEVAL)|
 | **output value** | **type** |
| an arbitrary function | scalar/vector/matrix/grid |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector/matrix/grid | the values input to this function |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the values input to this function |
| PERIODIC | compulsory | none | if the output of your function is periodic then you should specify the periodicity of the function |
| FUNC | compulsory | none | the function you wish to evaluate |
| VAR | optional | not used | the names to give each of the arguments in the function |

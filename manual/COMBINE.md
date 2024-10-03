# [Shortcut](shortcuts.md): COMBINE

| Description    | Usage |
|:--------|:--------:|
| Calculate a polynomial combination of a set of other variables. | [![used in 4 tutorials](https://img.shields.io/badge/tutorials-4-green.svg)](https://www.plumed-tutorials.org/browse.html?search=COMBINE)[![used in 81 eggs](https://img.shields.io/badge/nest-81-green.svg)](https://www.plumed-nest.org/browse.html?search=COMBINE)|
 | **output value** | **type** |
| a linear compbination | scalar/vector/matrix |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector/matrix | the values input to this function |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the values input to this function |
| PERIODIC | compulsory | none | if the output of your function is periodic then you should specify the periodicity of the function |
| COEFFICIENTS | compulsory | 1.0 |  the coefficients of the arguments in your function |
| PARAMETERS | compulsory | 0.0 |  the parameters of the arguments in your function |
| POWERS | compulsory | 1.0 |  the powers to which you are raising each of the arguments in your function |
| NORMALIZE | optional | false |  normalize all the coefficients so that in total they are equal to one |

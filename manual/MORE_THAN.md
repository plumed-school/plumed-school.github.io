# [Shortcut](shortcuts.md): MORE_THAN

| Description    | Usage |
|:--------|:--------:|
| Use a switching function to determine how many of the input variables are more than a certain cutoff. | [![used in 4 tutorials](https://img.shields.io/badge/tutorials-4-green.svg)](https://www.plumed-tutorials.org/browse.html?search=MORE_THAN)[![used in 23 eggs](https://img.shields.io/badge/nest-23-green.svg)](https://www.plumed-nest.org/browse.html?search=MORE_THAN)|
 | **output value** | **type** |
| a function that is one if the if the input is more than a threshold | scalar/vector/matrix |

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
| NN | compulsory | 6 |  The n parameter of the switching function  |
| MM | compulsory | 0 |  The m parameter of the switching function; 0 implies 2*NN |
| D_0 | compulsory | 0.0 |  The d_0 parameter of the switching function |
| R_0 | compulsory | none | The r_0 parameter of the switching function |
| SWITCH | optional | not used | This keyword is used if you want to employ an alternative to the continuous swiching function defined above |
| SQUARED | optional | false |  is the input quantity the square of the value that you would like to apply the switching function to |

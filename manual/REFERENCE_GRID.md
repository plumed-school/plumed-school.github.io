# Action: REFERENCE_GRID

| Description    | Usage |
|:--------|:--------:|
| Setup a constant grid by either reading values from a file or definining a function in input | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=REFERENCE_GRID)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the constant function on the grid that was specified in input | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| GRID_MIN | compulsory | none |  the lower bounds for the grid |
| GRID_MAX | compulsory | none |  the upper bounds for the grid |
| PERIODIC | compulsory | none | are the grid directions periodic |
| FILE | compulsory | none | the name of the file that contains the reference data |
| VALUE | compulsory | none | the name of the value that should be read from the grid |
| FUNC | optional | not used | the function to compute on the grid |
| GRID_BIN | optional | not used | the number of bins for the grid |
| GRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with GRID_BIN) |
| VAR | optional | not used | the names to give each of the grid directions in the function |

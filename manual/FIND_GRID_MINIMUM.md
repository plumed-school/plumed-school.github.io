# [Action](actions.md): FIND_GRID_MINIMUM

| Description    | Usage |
|:--------|:--------:|
| Find the point with the lowest value of the function on the grid | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| optval | scalar | the value of the function at the optimum | 
| _opt | scalar | the values of the arguments of the function at the optimum can be referenced elsewhere in the input file by using the names of the arguments followed by the string _opt | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | grid | the label for the function on the grid that you would like to find the optimum in |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label for the function on the grid that you would like to find the optimum in |
| CGTOL | compulsory | 1E-4 |  the tolerance for the conjugate gradient optimization |
| SERIAL | optional | false |  do the calculation in serial |
| NOINTERPOL | optional | false |  do not interpolate the function when finding the optimum |

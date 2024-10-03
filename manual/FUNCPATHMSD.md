# [Action](actions.md): FUNCPATHMSD

| Description    | Usage |
|:--------|:--------:|
| This function calculates path collective variables. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 5 eggs](https://img.shields.io/badge/nest-5-green.svg)](https://www.plumed-nest.org/browse.html?search=FUNCPATHMSD) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| s | scalar | the position on the path | 
| z | scalar | the distance from the path | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of the values from which the function is calculated |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the values from which the function is calculated |
| LAMBDA | compulsory | none | the lambda parameter is needed for smoothing, is in the units of plumed |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NEIGH_SIZE | optional | not used | size of the neighbor list |
| NEIGH_STRIDE | optional | not used | how often the neighbor list needs to be calculated in time units |

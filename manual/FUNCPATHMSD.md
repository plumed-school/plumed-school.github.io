# Action: FUNCPATHMSD

| Description    | Usage |
|:--------|:--------:|
| This function calculates path collective variables. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 5 eggs](https://img.shields.io/badge/nest-5-green.svg)](https://www.plumed-nest.org/browse.html?search=FUNCPATHMSD) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| s | scalar | the position on the path | 
| z | scalar | the distance from the path | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| LAMBDA | compulsory | none | the lambda parameter is needed for smoothing, is in the units of plumed |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NEIGH_SIZE | optional | not used | size of the neighbor list |
| NEIGH_STRIDE | optional | not used | how often the neighbor list needs to be calculated in time units |

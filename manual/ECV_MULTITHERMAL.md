# Action: ECV_MULTITHERMAL

| Description    | Usage |
|:--------|:--------:|
| Expand a simulation to sample multiple temperatures simultaneously. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=ECV_MULTITHERMAL)[![used in 9 eggs](https://img.shields.io/badge/nest-9-green.svg)](https://www.plumed-nest.org/browse.html?search=ECV_MULTITHERMAL) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the label of the internal energy of the system |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label of the internal energy of the system |
| TEMP | compulsory | none |  temperature |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| TEMP_MIN | optional | not used | the minimum of the temperature range |
| TEMP_MAX | optional | not used | the maximum of the temperature range |
| TEMP_STEPS | optional | not used | the number of steps in temperature |
| TEMP_SET_ALL | optional | not used | manually set all the temperatures |
| NO_GEOM_SPACING | optional | false |  do not use geometrical spacing in temperature, but instead linear spacing in inverse temperature |

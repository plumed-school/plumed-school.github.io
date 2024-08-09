# Action: ECV_MULTITHERMAL_MULTIBARIC

| Description    | Usage |
|:--------|:--------:|
| Expand a simulation to sample multiple temperatures and pressures. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=ECV_MULTITHERMAL_MULTIBARIC) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of the potential energy and of the volume of the system |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the potential energy and of the volume of the system |
| TEMP | compulsory | none |  temperature |
| PRESSURE | compulsory | none | pressure |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| TEMP_MIN | optional | not used | the minimum of the temperature range |
| TEMP_MAX | optional | not used | the maximum of the temperature range |
| TEMP_STEPS | optional | not used | the number of steps in temperature |
| TEMP_SET_ALL | optional | not used | manually set all the temperatures |
| NO_GEOM_SPACING | optional | false |  do not use geometrical spacing in temperature, but instead linear spacing in inverse temperature |
| PRESSURE_MIN | optional | not used | the minimum of the pressure range |
| PRESSURE_MAX | optional | not used | the maximum of the pressure range |
| PRESSURE_STEPS | optional | not used | the number of steps in pressure |
| PRESSURE_SET_ALL | optional | not used | manually set all the pressures |
| SET_ALL_TEMP_PRESSURE | optional | not used | manually set all the target temperature_pressure pairs |
| CUT_CORNER | optional | not used | avoid region of high temperature and low pressure |

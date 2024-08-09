# Action: ECV_LINEAR

| Description    | Usage |
|:--------|:--------:|
| Linear expansion, according to a parameter lambda. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=ECV_LINEAR) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the label of the Hamiltonian difference |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label of the Hamiltonian difference |
| TEMP | compulsory | none |  temperature |
| LAMBDA | compulsory | none |  the lambda at which the underlying simulation runs |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| LAMBDA_MIN | optional | not used |  the minimum of the lambda range |
| LAMBDA_MAX | optional | not used |  the maximum of the lambda range |
| LAMBDA_STEPS | optional | not used | uniformly place the lambda values, for a total of LAMBDA_STEPS |
| LAMBDA_SET_ALL | optional | not used | manually set all the lamdbas |
| DIMENSIONLESS | optional | false |  ARG is considered dimensionless rather than an energy, thus is not multiplied by beta |
| GEOM_SPACING | optional | false |  use geometrical spacing in lambda instead of linear spacing |

# Action: ECV_CUSTOM

| Description    | Usage |
|:--------|:--------:|
| Use some given CVs as a set of expansion collective variables (ECVs). | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of the single ECVs |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the single ECVs |
| TEMP | compulsory | none |  temperature |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ADD_P0 | optional | false |  add the unbiased Boltzmann distribution to the target distribution, to make sure to sample it |
| DIMENSIONLESS | optional | false |  consider ARG as dimensionless rather than an energy, thus do not multiply it by beta |
| BARRIER | optional | not used | a guess of the free energy barrier to be overcome (better to stay higher than lower) |

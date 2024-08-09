# Action: EXTERNAL

| Description    | Usage |
|:--------|:--------:|
| Calculate a restraint that is defined on a grid that is read during start up | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 8 eggs](https://img.shields.io/badge/nest-8-green.svg)](https://www.plumed-nest.org/browse.html?search=EXTERNAL) | 

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
| FILE | compulsory | none | the name of the file containing the external potential |
| SCALE | compulsory | none |  a factor that multiplies the external potential, useful to invert free energies |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOSPLINE | optional | false |  specifies that no spline interpolation is to be used when calculating the energy and forces due to the external potential |
| SPARSE | optional | false |  specifies that the external potential uses a sparse grid |

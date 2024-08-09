# Action: EEFSOLV

| Description    | Usage |
|:--------|:--------:|
| Calculates EEF1 solvation free energy for a group of atoms. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=EEFSOLV)|
 | **output value** | **type** |
| the EEF1 solvation free energy for the input atoms | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | The atoms to be included in the calculation, e |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | The atoms to be included in the calculation, e |
| NL_BUFFER | compulsory | none |  The buffer to the intrinsic cutoff used when calculating pairwise interactions |
| NL_STRIDE | compulsory | none |  The frequency with which the neighbor list is updated |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SERIAL | optional | false |  Perform the calculation in serial - for debug purpose |
| TEMP_CORRECTION | optional | false |  Correct free energy of solvation constants for temperatures different from 298 |

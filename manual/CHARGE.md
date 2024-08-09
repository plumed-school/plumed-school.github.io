# Action: CHARGE

| Description    | Usage |
|:--------|:--------:|
| Get the charges of one or multiple atoms | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=CHARGE)|
 | **output value** | **type** |
| the CHARGE of the atom | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOM | atoms | the atom number |
| ATOMS | atoms | the atom numbers that you would like to store the masses and charges of |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOM | input | none | the atom number |
| ATOMS | input | none | the atom numbers that you would like to store the masses and charges of |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |

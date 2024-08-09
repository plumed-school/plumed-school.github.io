# Action: GHBFIX

| Description    | Usage |
|:--------|:--------:|
| Calculate the GHBFIX interaction energy among GROUPA and GROUPB | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 3 eggs](https://img.shields.io/badge/nest-3-green.svg)](https://www.plumed-nest.org/browse.html?search=GHBFIX)|
 | **output value** | **type** |
| the GHBFIX interaction energy between the atoms in GROUPA and GROUPB | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| GROUPA | atoms | First list of atoms |
| GROUPB | atoms | Second list of atoms (if empty, N*(N-1)/2 pairs in GROUPA are counted) |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| GROUPA | input | none | First list of atoms |
| GROUPB | input | none | Second list of atoms (if empty, N*(N-1)/2 pairs in GROUPA are counted) |
| TYPES | compulsory | none | the value of TYPES in the switching function |
| PARAMS | compulsory | none | the value of PARAMS in the switching function |
| D_MAX | compulsory | none | the value of D_MAX in the switching function |
| D_0 | compulsory | none | the value of D_0 in the switching function |
| C | compulsory | none | the value of C in the switching function |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SERIAL | optional | false |  Perform the calculation in serial - for debug purpose |
| PAIR | optional | false |  Pair only 1st element of the 1st group with 1st element in the second, etc |
| NLIST | optional | false |  Use a neighbor list to speed up the calculation |
| NL_CUTOFF | optional | not used | The cutoff for the neighbor list |
| NL_STRIDE | optional | not used | The frequency with which we are updating the atoms in the neighbor list |
| ENERGY_UNITS | optional | not used | the value of ENERGY_UNITS in the switching function |

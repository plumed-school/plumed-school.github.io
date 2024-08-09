# Action: SASA_LCPO

| Description    | Usage |
|:--------|:--------:|
| Calculates the solvent accessible surface area (SASA) of a protein molecule, or other properties related to it. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the solvent accessible surface area (SASA) of the molecule | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the group of atoms that you are calculating the SASA for |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the group of atoms that you are calculating the SASA for |
| TYPE | compulsory | none |  The type of calculation you want to perform |
| NL_STRIDE | compulsory | none | The frequency with which the neighbor list is updated |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| DELTAGFILE | optional | not used | a file containing the free energy values for backbone and sidechains |
| APPROACH | optional | not used | either approach 2 or 3 |

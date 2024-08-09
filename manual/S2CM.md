# Action: S2CM

| Description    | Usage |
|:--------|:--------:|
| S2 contact model CV. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the value of the CV | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| METHYL_ATOM | atoms | the methyl carbon atom of the residue (i) |
| NH_ATOMS | atoms | the hydrogen atom of the NH group of the residue (i) and carbonyl oxygen of the preceding residue (i-1) |
| HEAVY_ATOMS | atoms | the heavy atoms to be included in the calculation |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| METHYL_ATOM | input | none | the methyl carbon atom of the residue (i) |
| NH_ATOMS | input | none | the hydrogen atom of the NH group of the residue (i) and carbonyl oxygen of the preceding residue (i-1) |
| HEAVY_ATOMS | input | none | the heavy atoms to be included in the calculation |
| R_EFF | compulsory | none | the effective distance, r_eff in the equation, given in nm |
| PREFACTOR_A | compulsory | none | the prefactor, a in the equation |
| EXPONENT_B | compulsory | none | the exponent, b in the equation |
| OFFSET_C | compulsory | none | the offset, c in the equation |
| N_I | compulsory | none |  n_i in the equation |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SERIAL | optional | false |  Perform the calculation in serial - for debug purpose |
| NLIST | optional | false |  Use a neighbour list to speed up the calculation |
| NL_CUTOFF | optional | not used | The cutoff for the neighbour list |
| NL_STRIDE | optional | not used | The frequency with which we are updating the atoms in the neighbour list |
| R_SHIFT | optional | not used | shift all distances by given amount |

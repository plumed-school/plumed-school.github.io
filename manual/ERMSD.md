# Action: ERMSD

| Description    | Usage |
|:--------|:--------:|
| Calculate eRMSD with respect to a reference structure. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 8 eggs](https://img.shields.io/badge/nest-8-green.svg)](https://www.plumed-nest.org/browse.html?search=ERMSD)|
 | **output value** | **type** |
| the eRMSD between the instantaneous structure and the reference structure that was input | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the list of atoms (use lcs) |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the list of atoms (use lcs) |
| REFERENCE | compulsory | none | a file in pdb format containing the reference structure and the atoms involved in the CV |
| CUTOFF | compulsory | none |  only pairs of atoms closer than CUTOFF are considered in the calculation |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| PAIRS | optional | not used | List of pairs considered |

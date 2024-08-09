# Action: MULTI_RMSD

| Description    | Usage |
|:--------|:--------:|
| Calculate RMSD distances for different domains and combine them. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=MULTI_RMSD)|
 | **output value** | **type** |
| the sum of the multiple RMSD distances | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| REFERENCE | compulsory | none | a file in pdb format containing the reference structure and the atoms involved in the CV |
| TYPE | compulsory | none |  the manner in which RMSD alignment is performed |
| SQUARED | optional | false |   This should be set if you want the mean squared displacement instead of the root mean squared displacement |
| NOPBC | optional | false |  don't use periodic boundary conditions |

# Action: RMSD

| Description    | Usage |
|:--------|:--------:|
| Calculate the RMSD with respect to a reference structure. | [![used in 3 tutorials](https://img.shields.io/badge/tutorials-3-green.svg)](https://www.plumed-tutorials.org/browse.html?search=RMSD)[![used in 29 eggs](https://img.shields.io/badge/nest-29-green.svg)](https://www.plumed-nest.org/browse.html?search=RMSD)|
 | **output value** | **type** |
| the RMSD distance between the instaneous structure and the reference structure/s that were input | scalar |

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
| NUMBER | compulsory | none |  if there are multiple structures in the pdb file you can specify that you want the RMSD from a specific structure by specifying its place in the file here |
| SQUARED | optional | false |   This should be setted if you want MSD instead of RMSD  |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| DISPLACEMENT | optional | false |  Calculate the vector of displacements instead of the length of this vector |

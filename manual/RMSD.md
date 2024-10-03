# [Shortcut](shortcuts.md): RMSD

| Description    | Usage |
|:--------|:--------:|
| Calculate the RMSD with respect to a reference structure. | [![used in 4 tutorials](https://img.shields.io/badge/tutorials-4-green.svg)](https://www.plumed-tutorials.org/browse.html?search=RMSD)[![used in 30 eggs](https://img.shields.io/badge/nest-30-green.svg)](https://www.plumed-nest.org/browse.html?search=RMSD)|
 | **output value** | **type** |
| the RMSD distance between the instaneous structure and the reference structure/s that were input | scalar/vector |

## Output components

This action can calculate the [values](pecifying_arguments.html) in the following table when the associated keyword is included in the input for the action. These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| disp | vector/matrix | DISPLACEMENT | the vector of displacements for the atoms | 
| dist | scalar/vector | DISPLACEMENT | the RMSD distance the atoms have moved | 


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| REFERENCE | compulsory | none | a file in pdb format containing the reference structure and the atoms involved in the CV |
| TYPE | compulsory | SIMPLE |  the manner in which RMSD alignment is performed |
| NUMBER | compulsory | 0 |  if there are multiple structures in the pdb file you can specify that you want the RMSD from a specific structure by specifying its place in the file here |
| SQUARED | optional | false |   This should be setted if you want MSD instead of RMSD  |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| DISPLACEMENT | optional | false |  Calculate the vector of displacements instead of the length of this vector |

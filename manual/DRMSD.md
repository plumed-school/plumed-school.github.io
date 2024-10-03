# [Shortcut](shortcuts.md): DRMSD

| Description    | Usage |
|:--------|:--------:|
| Calculate the distance RMSD with respect to a reference structure. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=DRMSD)|
 | **output value** | **type** |
| the DRMSD distance between the instantaneous structure and the reference structure | scalar/vector |

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| REFERENCE | compulsory | none | a file in pdb format containing the reference structure and the atoms involved in the CV |
| TYPE | compulsory | DRMSD |  what kind of DRMSD would you like to calculate |
| LOWER_CUTOFF | optional | not used | only pairs of atoms further than LOWER_CUTOFF are considered in the calculation |
| UPPER_CUTOFF | optional | not used | only pairs of atoms closer than UPPER_CUTOFF are considered in the calculation |
| SQUARED | optional | false |  This should be setted if you want MSD instead of RMSD  |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |

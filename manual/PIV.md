# Action: PIV

| Description    | Usage |
|:--------|:--------:|
| Calculates the PIV-distance. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=PIV)|
 | **output value** | **type** |
| the PIV-distance | scalar |

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
| SWITCH | compulsory | none | The switching functions parameter |
| PRECISION | compulsory | none | the precision for approximating reals with integers in sorting |
| REF_FILE | compulsory | none | PDB file name that contains the ith reference structure |
| PIVATOMS | compulsory | none | Number of atoms to use for PIV |
| SORT | compulsory | none | Whether to sort or not the PIV block |
| ATOMTYPES | compulsory | none | The atom types to use for PIV |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SFACTOR | optional | not used | Scale the PIV-distance by such block-specific factor |
| VOLUME | optional | not used | Scale atom-atom distances by the cubic root of the cell volume |
| UPDATEPIV | optional | not used | Frequency (in steps) at which the PIV is updated |
| TEST | optional | false |  Print the actual and reference PIV and exit |
| COM | optional | false |  Use centers of mass of groups of atoms instead of atoms as specified in the Pdb file |
| ONLYCROSS | optional | false |  Use only cross-terms (A-B, A-C, B-C,  |
| ONLYDIRECT | optional | false |  Use only direct-terms (A-A, B-B, C-C,  |
| DERIVATIVES | optional | false |  Activate the calculation of the PIV for every class (needed for numerical derivatives) |
| NLIST | optional | false |  Use a neighbor list for distance calculations |
| SERIAL | optional | false |  Perform the calculation in serial - for debug purpose |
| TIMER | optional | false |  Perform timing analysis on heavy loops |
| NL_CUTOFF | optional | not used | Neighbor lists cutoff |
| NL_STRIDE | optional | not used | Update neighbor lists every NL_STRIDE steps |
| NL_SKIN | optional | not used | The maximum atom displacement tolerated for the neighbor lists update |

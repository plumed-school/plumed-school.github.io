# Action: PARABETARMSD

| Description    | Usage |
|:--------|:--------:|
| Probe the parallel beta sheet content of your protein structure. | [![used in 3 tutorials](https://img.shields.io/badge/tutorials-3-green.svg)](https://www.plumed-tutorials.org/browse.html?search=PARABETARMSD)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=PARABETARMSD) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| struct | scalar | the vectors containing the rmsd distances between the residues and each of the reference structures | 
| lessthan | scalar | the number blocks of residues that have an RMSD from the secondary structure that is less than the threshold | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| RESIDUES | atoms | this command is used to specify the set of residues that could conceivably form part of the secondary structure |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| RESIDUES | input | none | this command is used to specify the set of residues that could conceivably form part of the secondary structure |
| TYPE | compulsory | none |  the manner in which RMSD alignment is performed |
| D_0 | compulsory | none |  The d_0 parameter of the switching function |
| NN | compulsory | none |  The n parameter of the switching function |
| MM | compulsory | none |  The m parameter of the switching function |
| STYLE | compulsory | none |  Parallel beta sheets can either form in a single chain or from a pair of chains |
| SERIAL | optional | false |  do the calculation in serial |
| NOPBC | optional | false |  ignore the periodic boundary conditions |
| STRANDS_CUTOFF | optional | not used | If in a segment of protein the two strands are further apart then the calculation of the actual RMSD is skipped as the structure is very far from being beta-sheet like |
| VERBOSE | optional | false |  write a more detailed output |
| LESS_THAN | optional | not used | calculate the number of a residue segments that are within a certain target distance of this secondary structure type |
| R_0 | optional | not used | The r_0 parameter of the switching function |

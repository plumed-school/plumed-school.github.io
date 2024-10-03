# [Action](actions.md): SECONDARY_STRUCTURE_RMSD

| Description    | Usage |
|:--------|:--------:|
| Calclulate the distance between segments of a protein and a reference structure of interest | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=SECONDARY_STRUCTURE_RMSD)[![used in 16 eggs](https://img.shields.io/badge/nest-16-green.svg)](https://www.plumed-nest.org/browse.html?search=SECONDARY_STRUCTURE_RMSD)|
 | **output value** | **type** |
| a vector containing the rmsd distance between each of the residue segments and the reference structure | vector |

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| struct | vector | the vectors containing the rmsd distances between the residues and each of the reference structures | 
| lessthan | scalar | the number blocks of residues that have an RMSD from the secondary structure that is less than the threshold | 


## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| RESIDUES | atoms | this command is used to specify the set of residues that could conceivably form part of the secondary structure |
| ATOMS | atoms | this is the full list of atoms that we are investigating |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| RESIDUES | input | none | this command is used to specify the set of residues that could conceivably form part of the secondary structure |
| ATOMS | input | none | this is the full list of atoms that we are investigating |
| BONDLENGTH | compulsory | none | the length to use for bonds |
| TYPE | compulsory | DRMSD |  the manner in which RMSD alignment is performed |
| D_0 | compulsory | 0.0 |  The d_0 parameter of the switching function |
| NN | compulsory | 8 |  The n parameter of the switching function |
| MM | compulsory | 12 |  The m parameter of the switching function |
| SERIAL | optional | false |  do the calculation in serial |
| NOPBC | optional | false |  ignore the periodic boundary conditions |
| SEGMENT | optional | not used | this is the lists of atoms in the segment that are being considered |
| STRUCTURE | optional | not used | the reference structure |
| STRANDS_CUTOFF | optional | not used | If in a segment of protein the two strands are further apart then the calculation of the actual RMSD is skipped as the structure is very far from being beta-sheet like |
| CUTOFF_ATOMS | optional | not used | the pair of atoms that are used to calculate the strand cutoff |
| VERBOSE | optional | false |  write a more detailed output |
| LESS_THAN | optional | not used | calculate the number of a residue segments that are within a certain target distance of this secondary structure type |
| R_0 | optional | not used | The r_0 parameter of the switching function |

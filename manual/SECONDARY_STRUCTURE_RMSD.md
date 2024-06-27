# Action: SECONDARY_STRUCTURE_RMSD

| Description    | Usage |
|:--------:|:--------:|
| Calclulate the distance between segments of a protein and a reference structure of interest | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://plumed-school.github.io/browse.html?search=SECONDARY_STRUCTURE_RMSD)[![used in 15 eggs](https://img.shields.io/badge/nest-15-green.svg)](https://www.plumed-nest.org/browse.html?search=SECONDARY_STRUCTURE_RMSD) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| RESIDUES | input | none | this command is used to specify the set of residues that could conceivably form part of the secondary structure |
| ATOMS | input | none | this is the full list of atoms that we are investigating |
| BONDLENGTH | compulsory | none | the length to use for bonds |
| TYPE | compulsory | none |  the manner in which RMSD alignment is performed |
| D_0 | compulsory | none |  The d_0 parameter of the switching function |
| NN | compulsory | none |  The n parameter of the switching function |
| MM | compulsory | none |  The m parameter of the switching function |
| SERIAL | optional | false |  do the calculation in serial |
| NOPBC | optional | false |  ignore the periodic boundary conditions |
| SEGMENT | optional | not used | this is the lists of atoms in the segment that are being considered |
| STRUCTURE | optional | not used | the reference structure |
| STRANDS_CUTOFF | optional | not used | If in a segment of protein the two strands are further apart then the calculation of the actual RMSD is skipped as the structure is very far from being beta-sheet like |
| CUTOFF_ATOMS | optional | not used | the pair of atoms that are used to calculate the strand cutoff |
| VERBOSE | optional | false |  write a more detailed output |
| LESS_THAN | optional | not used | calculate the number of a residue segments that are within a certain target distance of this secondary structure type |
| R_0 | optional | not used | The r_0 parameter of the switching function |

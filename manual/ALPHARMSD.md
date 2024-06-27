# Action: ALPHARMSD

| Description    | Usage |
|:--------:|:--------:|
| Probe the alpha helical content of a protein structure. | [![used in 3 tutorials](https://img.shields.io/badge/tutorials-3-green.svg)](https://plumed-school.github.io/browse.html?search=ALPHARMSD)[![used in 14 eggs](https://img.shields.io/badge/nest-14-green.svg)](https://www.plumed-nest.org/browse.html?search=ALPHARMSD) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| RESIDUES | input | none | this command is used to specify the set of residues that could conceivably form part of the secondary structure |
| TYPE | compulsory | none |  the manner in which RMSD alignment is performed |
| D_0 | compulsory | none |  The d_0 parameter of the switching function |
| NN | compulsory | none |  The n parameter of the switching function |
| MM | compulsory | none |  The m parameter of the switching function |
| SERIAL | optional | false |  do the calculation in serial |
| NOPBC | optional | false |  ignore the periodic boundary conditions |
| VERBOSE | optional | false |  write a more detailed output |
| LESS_THAN | optional | not used | calculate the number of a residue segments that are within a certain target distance of this secondary structure type |
| R_0 | optional | not used | The r_0 parameter of the switching function |

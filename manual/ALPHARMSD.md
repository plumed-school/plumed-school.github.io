# [Action](actions.md): ALPHARMSD

| Description    | Usage |
|:--------|:--------:|
| Probe the alpha helical content of a protein structure. | [![used in 3 tutorials](https://img.shields.io/badge/tutorials-3-green.svg)](https://www.plumed-tutorials.org/browse.html?search=ALPHARMSD)[![used in 15 eggs](https://img.shields.io/badge/nest-15-green.svg)](https://www.plumed-nest.org/browse.html?search=ALPHARMSD)|
 | **output value** | **type** |
| if LESS_THAN is present the RMSD distance between each residue and the ideal alpha helix | scalar/vector |

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


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| RESIDUES | input | none | this command is used to specify the set of residues that could conceivably form part of the secondary structure |
| TYPE | compulsory | DRMSD |  the manner in which RMSD alignment is performed |
| D_0 | compulsory | 0.0 |  The d_0 parameter of the switching function |
| NN | compulsory | 8 |  The n parameter of the switching function |
| MM | compulsory | 12 |  The m parameter of the switching function |
| SERIAL | optional | false |  do the calculation in serial |
| NOPBC | optional | false |  ignore the periodic boundary conditions |
| VERBOSE | optional | false |  write a more detailed output |
| LESS_THAN | optional | not used | calculate the number of a residue segments that are within a certain target distance of this secondary structure type |
| R_0 | optional | not used | The r_0 parameter of the switching function |

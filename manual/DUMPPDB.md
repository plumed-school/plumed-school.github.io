# Action: DUMPPDB

| Description    | Usage |
|:--------|:--------:|
| Output PDB file. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=DUMPPDB)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| STRIDE | compulsory | none |  the frequency with which the atoms should be output |
| FILE | compulsory | none | the name of the file on which to output these quantities |
| FMT | compulsory | none |  the format that should be used to output real numbers |
| OCCUPANCY | compulsory | none |  vector of values to output in the occupancy column of the pdb file |
| BETA | compulsory | none |  vector of values to output in the beta column of the pdb file |
| ATOMS | optional | not used | value containing positions of atoms that should be output |
| DESCRIPTION | optional | not used | the title to use for your PDB output |
| ATOM_INDICES | optional | not used | the indices of the atoms in your PDB output |
| ARG_NAMES | optional | not used | the names of the arguments that are being output |

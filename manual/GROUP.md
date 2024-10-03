# [Action](actions.md): GROUP

| Description    | Usage |
|:--------|:--------:|
| Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. | [![used in 11 tutorials](https://img.shields.io/badge/tutorials-11-green.svg)](https://www.plumed-tutorials.org/browse.html?search=GROUP)[![used in 117 eggs](https://img.shields.io/badge/nest-117-green.svg)](https://www.plumed-nest.org/browse.html?search=GROUP) | 

## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the numerical indexes for the set of atoms in the group |
| REMOVE | atoms | remove these atoms from the list |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the numerical indexes for the set of atoms in the group |
| REMOVE | input | none | remove these atoms from the list |
| SORT | optional | false |  sort the resulting list |
| UNIQUE | optional | false |  sort atoms and remove duplicated ones |
| NDX_FILE | optional | not used | the name of index file (gromacs syntax) |
| NDX_GROUP | optional | not used | the name of the group to be imported (gromacs syntax) - first group found is used by default |

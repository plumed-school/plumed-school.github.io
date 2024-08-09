# Action: WHOLEMOLECULES

| Description    | Usage |
|:--------|:--------:|
| This action is used to rebuild molecules that can become split by the periodic boundary conditions. | [![used in 3 tutorials](https://img.shields.io/badge/tutorials-3-green.svg)](https://www.plumed-tutorials.org/browse.html?search=WHOLEMOLECULES)[![used in 118 eggs](https://img.shields.io/badge/nest-118-green.svg)](https://www.plumed-nest.org/browse.html?search=WHOLEMOLECULES) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ENTITY | atoms | the atoms that make up a molecule that you wish to align |
| RESIDUES | atoms | this command specifies that the backbone atoms in a set of residues all must be aligned |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ENTITY | input | none | the atoms that make up a molecule that you wish to align |
| RESIDUES | input | none | this command specifies that the backbone atoms in a set of residues all must be aligned |
| STRIDE | compulsory | none |  the frequency with which molecules are reassembled |
| MOLTYPE | optional | not used | the type of molecule that is under study |
| EMST | optional | false |  Define atoms sequence in entities using an Euclidean minimum spanning tree |
| ADDREFERENCE | optional | false |  Define the reference position of the first atom of each entity using a PDB file |

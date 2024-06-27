# Action: PDB2CONSTANT

| Description    | Usage |
|:--------:|:--------:|
| Create a constant value from a PDB input file | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://plumed-school.github.io/browse.html?search=PDB2CONSTANT)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=PDB2CONSTANT) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | read this single argument from the input rather than the atomic structure |
| REFERENCE | compulsory | none | a file in pdb format containing the reference structure |
| NUMBER | compulsory | none |  if there are multiple structures in the pdb file you can specify that you want the RMSD from a specific structure by specifying its place in the file here |
| NOARGS | optional | false |  the arguments that are being read from the PDB file are not in the plumed input |
| ARG | optional | not used | read this single argument from the input rather than the atomic structure |

# [Action](actions.md): MOLINFO

| Description    | Usage |
|:--------|:--------:|
| This command is used to provide information on the molecules that are present in your system. | [![used in 11 tutorials](https://img.shields.io/badge/tutorials-11-green.svg)](https://www.plumed-tutorials.org/browse.html?search=MOLINFO)[![used in 90 eggs](https://img.shields.io/badge/nest-90-green.svg)](https://www.plumed-nest.org/browse.html?search=MOLINFO) | 

## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| CHAIN | atoms | (for masochists ( mostly Davide Branduardi ) ) The atoms involved in each of the chains of interest in the structure |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| CHAIN | input | none | (for masochists ( mostly Davide Branduardi ) ) The atoms involved in each of the chains of interest in the structure |
| STRUCTURE | compulsory | none | a file in pdb format containing a reference structure |
| MOLTYPE | compulsory | protein |  what kind of molecule is contained in the pdb file - usually not needed since protein/RNA/DNA are compatible |
| PYTHON_BIN | compulsory | default |  python interpreter |
| WHOLE | optional | false |  The reference structure is whole, i |

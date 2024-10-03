# [Action](actions.md): DUMPATOMS

| Description    | Usage |
|:--------|:--------:|
| Dump selected atoms on a file. | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=DUMPATOMS)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=DUMPATOMS) | 

## Input

The [arguments](specifying_arguments.html) and [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | vector | the labels of vectors that should be output in the xyz file |
| ATOMS | atoms | the atom indices whose positions you would like to print out |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of vectors that should be output in the xyz file |
| ATOMS | input | none | the atom indices whose positions you would like to print out |
| STRIDE | compulsory | 1 |  the frequency with which the atoms should be output |
| FILE | compulsory | none | file on which to output coordinates; extension is automatically detected |
| UNITS | compulsory | PLUMED |  the units in which to print out the coordinates |
| PRECISION | optional | not used | The number of digits in trajectory file |
| TYPE | optional | not used | file type, either xyz, gro, xtc, or trr, can override an automatically detected file extension |
| LESS_THAN_OR_EQUAL | optional | not used | when printing with arguments that are vectors only print components of vectors have a value less than or equal to this value |
| GREATER_THAN_OR_EQUAL | optional | not used | when printing with arguments that are vectors only print components of vectors have a value greater than or equal to this value |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

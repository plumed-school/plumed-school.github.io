# [Action](actions.md): FIXEDATOM

| Description    | Usage |
|:--------|:--------:|
| Add a virtual atom in a fixed position. | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=FIXEDATOM)[![used in 17 eggs](https://img.shields.io/badge/nest-17-green.svg)](https://www.plumed-nest.org/browse.html?search=FIXEDATOM) | 

## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the list of atoms which are involved the virtual atom's definition |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the list of atoms which are involved the virtual atom's definition |
| AT | compulsory | none | coordinates of the virtual atom |
| SET_MASS | compulsory | 1 |  mass of the virtual atom |
| SET_CHARGE | compulsory | 0 |  charge of the virtual atom |
| SCALED_COMPONENTS | optional | false |  use scaled components |

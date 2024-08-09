# Action: FIXEDATOM

| Description    | Usage |
|:--------|:--------:|
| Add a virtual atom in a fixed position. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=FIXEDATOM)[![used in 17 eggs](https://img.shields.io/badge/nest-17-green.svg)](https://www.plumed-nest.org/browse.html?search=FIXEDATOM) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the list of atoms which are involved the virtual atom's definition |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the list of atoms which are involved the virtual atom's definition |
| AT | compulsory | none | coordinates of the virtual atom |
| SET_MASS | compulsory | none |  mass of the virtual atom |
| SET_CHARGE | compulsory | none |  charge of the virtual atom |
| SCALED_COMPONENTS | optional | false |  use scaled components |

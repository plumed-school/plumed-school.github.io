# Action: COM

| Description    | Usage |
|:--------|:--------:|
| Calculate the center of mass for a group of atoms. | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=COM)[![used in 59 eggs](https://img.shields.io/badge/nest-59-green.svg)](https://www.plumed-nest.org/browse.html?search=COM) | 

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
| WEIGHTS | optional | not used | Center is computed as a weighted average |
| SET_CHARGE | optional | not used | Set the charge of the virtual atom to a given value |
| SET_MASS | optional | not used | Set the mass of the virtual atom to a given value |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| MASS | optional | false |  If set center is mass weighted |
| PHASES | optional | false |  Compute center using trigonometric phases |

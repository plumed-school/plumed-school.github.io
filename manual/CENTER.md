# Action: CENTER

| Description    | Usage |
|:--------|:--------:|
| Calculate the center for a group of atoms, with arbitrary weights. | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=CENTER)[![used in 60 eggs](https://img.shields.io/badge/nest-60-green.svg)](https://www.plumed-nest.org/browse.html?search=CENTER)|
 | **output value** | **type** |
| the position of the center of mass | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the group of atoms that you are calculating the Gyration Tensor for |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the group of atoms that you are calculating the Gyration Tensor for |
| TYPE | compulsory | none |  The type of calculation relative to the Gyration Tensor you want to perform |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| WEIGHTS | optional | not used | what weights should be used when calculating the center |
| PHASES | optional | false |  use trigonometric phases when computing position of center |
| SAFE_PHASES | optional | false |  use trignomentric phases when computing position of center but also compute the center in ths usual way and use this when the pbc are not set |
| MASS | optional | false |  calculate the center of mass |

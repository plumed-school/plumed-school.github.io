# Action: GYRATION_TENSOR

| Description    | Usage |
|:--------|:--------:|
| Calculate the gyration tensor using a user specified vector of weights | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the radius that was computed from the weights | scalar |

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
| PHASES | optional | false |  use trigonometric phases when computing position of center of mass |
| MASS | optional | false |  calculate the center of mass |
| MASS_WEIGHTED | optional | false |  set the masses of all the atoms equal to one |
| UNORMALIZED | optional | false |  do not divide by the sum of the weights |

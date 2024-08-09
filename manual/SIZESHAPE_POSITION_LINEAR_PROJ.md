# Action: SIZESHAPE_POSITION_LINEAR_PROJ

| Description    | Usage |
|:--------|:--------:|
| Calculates a linear projection in the space of a given reference configurational distribution in size-and-shape space. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the linear projection | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| GROUP | atoms | Group of atoms being used |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| GROUP | input | none | Group of atoms being used |
| PRECISION | compulsory | none | Precision Matrix (inverse of covariance) |
| REFERENCE | compulsory | none | Coordinates of the reference structure |
| COEFFS | compulsory | none | Vector of linear coefficients |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SERIAL | optional | false |  Perform the calculation in serial, for debug purposes only |

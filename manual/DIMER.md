# Action: DIMER

| Description    | Usage |
|:--------|:--------:|
| This CV computes the dimer interaction energy for a collection of dimers. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the dimer interaction energy | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS1 | atoms | The list of atoms representing the first bead of each Dimer being considered by this CV |
| ATOMS2 | atoms | The list of atoms representing the second bead of each Dimer being considered by this CV |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS1 | input | none | The list of atoms representing the first bead of each Dimer being considered by this CV |
| ATOMS2 | input | none | The list of atoms representing the second bead of each Dimer being considered by this CV |
| DSIGMA | compulsory | none | The interaction strength of the dimer bond |
| Q | compulsory | none | The exponent of the dimer potential |
| TEMP | compulsory | none | The temperature (in Kelvin) of the simulation |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| ALLATOMS | optional | false |  Use EVERY atom of the system |
| NOVSITES | optional | false |  If present the configuration is without virtual sites at the centroid positions |

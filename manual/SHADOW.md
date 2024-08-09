# Action: SHADOW

| Description    | Usage |
|:--------|:--------:|
| Communicate atoms positions among replicas and calculate the RMSD with respect to a mother (reference) simulation. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=SHADOW)|
 | **output value** | **type** |
| the value of the shadow RMSD | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | atoms for which we calculate the shadow RMSD |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | atoms for which we calculate the shadow RMSD |
| UPDATE | compulsory | none | stride for updating reference coordinates |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| REFERENCE | optional | false |  this is the reference replica |

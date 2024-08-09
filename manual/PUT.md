# Action: PUT

| Description    | Usage |
|:--------|:--------:|
| Pass data into PLUMED | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=PUT)|
 | **output value** | **type** |
| the data that was passed from the MD code | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| SHAPE | compulsory | none |  the shape of the value that is being passed to PLUMED |
| UNIT | compulsory | none | the unit of the quantity that is being passed to PLUMED through this value |
| FORCE_UNIT | compulsory | none |  the units to use for the force |
| PERIODIC | compulsory | none | if the value being passed to plumed is periodic then you should specify the periodicity of the function |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ROLE | optional | not used | Get the role this value plays in the code can be x/y/z/m/q to signify that this is x, y, z positions of atoms or masses or charges of atoms |
| CONSTANT | optional | false |  does this quantity not depend on time |
| FROM_DOMAINS | optional | false |  is this quantity passed through the domain decomposition object |
| MUTABLE | optional | false |  can plumed change the value of the pointer that is passed from the MD code |

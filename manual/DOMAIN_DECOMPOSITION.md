# Action: DOMAIN_DECOMPOSITION

| Description    | Usage |
|:--------|:--------:|
| Pass domain decomposed properties of atoms to PLUMED | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=DOMAIN_DECOMPOSITION)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the domain that each atom is within | scalar |

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
| NATOMS | compulsory | none | the number of atoms across all the domains |
| PBCLABEL | compulsory | none |  the label to use for the PBC action that will be created |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| VALUE | optional | not used | value to create for the domain decomposition |
| UNIT | optional | not used | unit of the ith value that is being passed through the domain decomposition |
| CONSTANT | optional | not used | is the ith value that is being passed through the domain decomposition constant |
| PERIODIC | optional | not used | if the value being passed to plumed is periodic then you should specify the periodicity of the function |
| ROLE | optional | not used | Get the role this value plays in the code can be x/y/z/m/q to signify that this is x, y, z positions of atoms or masses or charges of atoms |

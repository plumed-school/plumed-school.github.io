# [Action](actions.md): CONTACTMAP

| Description    | Usage |
|:--------|:--------:|
| Calculate the distances between a number of pairs of atoms and transform each distance by a switching function. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 18 eggs](https://img.shields.io/badge/nest-18-green.svg)](https://www.plumed-nest.org/browse.html?search=CONTACTMAP)|
 | **output value** | **type** |
| the sum of all the switching function on all the distances | scalar |

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| contact | scalar | By not using SUM or CMDIST each contact will be stored in a component | 


## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the atoms involved in each of the contacts you wish to calculate |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the atoms involved in each of the contacts you wish to calculate |
| SWITCH | compulsory | none | The switching functions to use for each of the contacts in your map |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| REFERENCE | optional | not used | A reference value for a given contact, by default is 0 |
| WEIGHT | optional | not used | A weight value for a given contact, by default is 1 |
| SUM | optional | false |  calculate the sum of all the contacts in the input |
| CMDIST | optional | false |  calculate the distance with respect to the provided reference contact map |
| SERIAL | optional | false |  Perform the calculation in serial - for debug purpose |

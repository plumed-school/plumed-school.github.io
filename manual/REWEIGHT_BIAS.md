# [Action](actions.md): REWEIGHT_BIAS

| Description    | Usage |
|:--------|:--------:|
| Calculate weights for ensemble averages that negate the effect the bias has on the region of phase space explored | [![used in 5 tutorials](https://img.shields.io/badge/tutorials-5-green.svg)](https://www.plumed-tutorials.org/browse.html?search=REWEIGHT_BIAS)[![used in 13 eggs](https://img.shields.io/badge/nest-13-green.svg)](https://www.plumed-nest.org/browse.html?search=REWEIGHT_BIAS)|
 | **output value** | **type** |
| the weight to use for this frame to negate the effect the bias | scalar |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar |  the biases that must be taken into account when reweighting |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none |  the biases that must be taken into account when reweighting |
| TEMP | optional | not used | the system temperature |

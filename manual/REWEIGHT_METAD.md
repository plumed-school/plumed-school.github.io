# [Action](actions.md): REWEIGHT_METAD

| Description    | Usage |
|:--------|:--------:|
| Calculate the weights configurations should contribute to the histogram in a simulation in which a metadynamics bias acts upon the system. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=REWEIGHT_METAD)[![used in 16 eggs](https://img.shields.io/badge/nest-16-green.svg)](https://www.plumed-nest.org/browse.html?search=REWEIGHT_METAD)|
 | **output value** | **type** |
| the weight to use for this frame to negate the effect the metadynamics bias | scalar |

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

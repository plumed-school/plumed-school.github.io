# [Action](actions.md): REWEIGHT_TEMP_PRESS

| Description    | Usage |
|:--------|:--------:|
| Calculate weights for ensemble averages at temperatures and/or pressures different than those used in your original simulation. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 3 eggs](https://img.shields.io/badge/nest-3-green.svg)](https://www.plumed-nest.org/browse.html?search=REWEIGHT_TEMP_PRESS)|
 | **output value** | **type** |
| the weight to use for this frame to determine its contribution at a different temperature/pressure | scalar |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ENERGY | scalar | Energy |
| VOLUME | scalar | Volume |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ENERGY | input | none | Energy |
| VOLUME | input | none | Volume |
| TEMP | optional | not used | the system temperature |
| REWEIGHT_PRESSURE | optional | not used | Reweighting pressure |
| PRESSURE | optional | not used | The system pressure |
| REWEIGHT_TEMP | optional | not used | Reweighting temperature |

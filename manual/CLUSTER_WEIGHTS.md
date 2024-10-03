# [Action](actions.md): CLUSTER_WEIGHTS

| Description    | Usage |
|:--------|:--------:|
| Setup a vector that has one for all the atoms that form part of the cluster of interest and that has zero for all other atoms. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=CLUSTER_WEIGHTS)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=CLUSTER_WEIGHTS)|
 | **output value** | **type** |
| vector with elements that are one if the atom of interest is part of the required cluster and zero otherwise | vector |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| CLUSTERS | vector | the label of the action that does the clustering |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| CLUSTERS | input | none | the label of the action that does the clustering |
| CLUSTER | compulsory | 1 |  which cluster would you like to look at 1 is the largest cluster, 2 is the second largest, 3 is the the third largest and so on |
| LOWMEM | optional | false |  this flag does nothing and is present only to ensure back-compatibility |

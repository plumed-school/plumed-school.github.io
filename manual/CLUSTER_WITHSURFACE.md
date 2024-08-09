# Action: CLUSTER_WITHSURFACE

| Description    | Usage |
|:--------|:--------:|
| Determine the atoms that are within a certain cutoff of the atoms in a cluster | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=CLUSTER_WITHSURFACE)|
 | **output value** | **type** |
| a vector that is one for those atoms that are within the cluster or that are within a cetain cutoff of one of the atoms in the cluster and zero otherwise | scalar |

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
| ATOMS | compulsory | none | the atoms that were used to calculate the matrix that was clustered |
| CLUSTERS | compulsory | none | the label of the action that does the clustering |
| CLUSTER | compulsory | none |  which cluster would you like to look at 1 is the largest cluster, 2 is the second largest, 3 is the the third largest and so on |
| RCUT_SURF | optional | not used |  |

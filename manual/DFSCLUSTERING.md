# Action: DFSCLUSTERING

| Description    | Usage |
|:--------|:--------:|
| Find the connected components of the matrix using the depth first search clustering algorithm. | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=DFSCLUSTERING)[![used in 7 eggs](https://img.shields.io/badge/nest-7-green.svg)](https://www.plumed-nest.org/browse.html?search=DFSCLUSTERING)|
 | **output value** | **type** |
| vector with length that is equal to the number of rows in the input matrix | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| MATRIX | optional | not used | the input matrix (can use ARG instead) |
| LOWMEM | optional | false |  this flag does nothing and is present only to ensure back-compatibility |

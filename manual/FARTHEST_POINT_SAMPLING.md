# [Action](actions.md): FARTHEST_POINT_SAMPLING

| Description    | Usage |
|:--------|:--------:|
| Select a set of landmarks using farthest point sampling. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a vector which has as many elements as there are rows in the input matrix of dissimilarities | vector |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | matrix | the input matrix |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input matrix |
| NZEROS | compulsory | none | the number of landmark points that you want to select |
| SEED | compulsory | 1234 |  a random number seed |
| MATRIX | optional | not used | the input matrix (can use ARG instead) |

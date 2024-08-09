# Action: MAHALANOBIS_DISTANCE

| Description    | Usage |
|:--------|:--------:|
| Calculate the mahalanobis distance between two points in CV space | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the Mahalanobis distances between the input vectors | scalar |

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
| ARG1 | compulsory | none | The point that we are calculating the distance from |
| ARG2 | compulsory | none | The point that we are calculating the distance to |
| METRIC | compulsory | none | The inverse covariance matrix that should be used when calculating the distance |
| SQUARED | optional | false |  The squared distance should be calculated |
| VON_MISSES | optional | false |  Compute the mahalanobis distance in a way that is more sympathetic to the periodic boundary conditions |

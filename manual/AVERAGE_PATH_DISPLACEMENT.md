# [Action](actions.md): AVERAGE_PATH_DISPLACEMENT

| Description    | Usage |
|:--------|:--------:|
| Accumulate the distances between the reference frames in the paths and the configurations visited | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| matrix containing the average displacement between the trajectory and each of the landmarks that makes up the path | matrix |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | matrix | the labels of the matrix that contains the vectors of displacements from each frame in the path |
| REFERENCE | vector | labels for actions that contain reference coordinates for each point on the path |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the matrix that contains the vectors of displacements from each frame in the path |
| REFERENCE | input | none | labels for actions that contain reference coordinates for each point on the path |
| METRIC | compulsory | none | the method to use for computing the displacement vectors between the reference frames |
| METRIC_COMPONENT | compulsory | none | if the final action in your metric contains multiple components this keyword is used to specify the component that should be used |
| STRIDE | compulsory | 1 |  the frequency with which the average displacements should be collected and added to the average displacements |
| HALFLIFE | compulsory | -1 |  the number of MD steps after which a previously measured path distance weighs only 50 percent in the average |
| CLEAR | compulsory | 0 |  the frequency with which to clear all the accumulated data |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |

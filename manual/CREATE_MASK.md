# [Action](actions.md): CREATE_MASK

| Description    | Usage |
|:--------|:--------:|
| Create a mask vector to use for landmark selection | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a vector of zeros and ones that is used that can be used to mask some of the elements in a time series | vector |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | vector | the label of the vector that you would like to construct a mask for |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label of the vector that you would like to construct a mask for |
| TYPE | compulsory | none | the way the zeros are supposed to be set |
| NZEROS | compulsory | none | the number of zeros that you want to put in the mask |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| SEED | optional | not used | the seed to use for the random number generator |

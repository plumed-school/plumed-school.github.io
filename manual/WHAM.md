# [Action](actions.md): WHAM

| Description    | Usage |
|:--------|:--------:|
| Calculate the weights for configurations using the weighted histogram analysis method. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the vector of WHAM weights to use for reweighting the elements in a time series | vector |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector/matrix | the stored values for the bias |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the stored values for the bias |
| MAXITER | compulsory | 1000 |  maximum number of iterations for WHAM algorithm |
| WHAMTOL | compulsory | 1e-10 |  threshold for convergence of WHAM algorithm |
| TEMP | optional | not used | the system temperature |

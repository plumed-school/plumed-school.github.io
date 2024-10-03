# [Action](actions.md): GATHER_REPLICAS

| Description    | Usage |
|:--------|:--------:|
| Create a vector that contains the copies of the input quantities from all replicas | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=GATHER_REPLICAS)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector/matrix/grid | the argument from the various replicas that you would like to gather |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the argument from the various replicas that you would like to gather |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |

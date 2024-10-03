# [Action](actions.md): GET

| Description    | Usage |
|:--------|:--------:|
| Get data from PLUMED for another code | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector/matrix/grid | the label of the value that you would like to GET |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label of the value that you would like to GET |
| STRIDE | compulsory | 1 |  the frequency with which the quantities of interest should be stored |
| TYPE | compulsory | value |  what do you want to collect for the value can be derivative/force |

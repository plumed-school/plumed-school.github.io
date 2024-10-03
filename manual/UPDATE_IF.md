# [Action](actions.md): UPDATE_IF

| Description    | Usage |
|:--------|:--------:|
| Conditional update of other actions. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of values that should be used to make the decision on whether to update or not |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of values that should be used to make the decision on whether to update or not |
| STRIDE | compulsory | 1 |  the frequency with which the quantities of interest should be output |
| END | optional | false |  end |
| LESS_THAN | optional | not used | upper bound |
| MORE_THAN | optional | not used | lower bound |

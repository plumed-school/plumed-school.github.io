# [Action](actions.md): DUMPPROJECTIONS

| Description    | Usage |
|:--------|:--------:|
| Dump the derivatives with respect to the input parameters for one or more objects (generally CVs, functions or biases). | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of the values whose gradients should be outpu |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the values whose gradients should be outpu |
| STRIDE | compulsory | 1 |  the frequency with which the derivatives should be output |
| FILE | compulsory | none | the name of the file on which to output the derivatives |
| FMT | compulsory | %15.10f |  the format with which the derivatives should be output |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

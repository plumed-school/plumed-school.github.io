# [Action](actions.md): DUMPFORCES

| Description    | Usage |
|:--------|:--------:|
| Dump the force acting on one of a values in a file. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=DUMPFORCES) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of the values whose forces should be output |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the values whose forces should be output |
| STRIDE | compulsory | 1 |  the frequency with which the forces should be output |
| FILE | compulsory | none | the name of the file on which to output the forces |
| FMT | compulsory | %15.10f |  the format with which the derivatives should be output |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

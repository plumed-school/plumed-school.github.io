# [Action](actions.md): DUMPVECTOR

| Description    | Usage |
|:--------|:--------:|
| Print a vector to a file | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=DUMPVECTOR)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | vector/matrix | the labels of vectors/matrices that should be output in the file |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of vectors/matrices that should be output in the file |
| STRIDE | compulsory | 0 |  the frequency with which the grid should be output to the file |
| FILE | compulsory | density |  the file on which to write the vetors |
| FMT | optional | not used | the format that should be used to output real numbers |
| PRINT_ONE_FILE | optional | false |  output vectors one after the other in a single file |

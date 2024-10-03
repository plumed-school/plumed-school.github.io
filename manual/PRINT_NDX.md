# [Action](actions.md): PRINT_NDX

| Description    | Usage |
|:--------|:--------:|
| Print an ndx file | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) and [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | vector | the labels of vectors that should be used when printind the NDX file |
| ATOMS | atoms | the list of atoms that have the corresponding arguments |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of vectors that should be used when printind the NDX file |
| ATOMS | input | none | the list of atoms that have the corresponding arguments |
| STRIDE | compulsory | 1 |  the frequency with which the quantities of interest should be output |
| FILE | optional | not used | the name of the file on which to output these quantities |
| LESS_THAN_OR_EQUAL | optional | not used | when printing with arguments that are vectors only print components of vectors have a value less than or equal to this value |
| GREATER_THAN_OR_EQUAL | optional | not used | when printing with arguments that are vectors only print components of vectors have a value greater than or equal to this value |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

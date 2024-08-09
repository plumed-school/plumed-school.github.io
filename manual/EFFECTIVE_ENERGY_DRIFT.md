# Action: EFFECTIVE_ENERGY_DRIFT

| Description    | Usage |
|:--------|:--------:|
| Print the effective energy drift | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=EFFECTIVE_ENERGY_DRIFT)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| STRIDE | compulsory | none |  should be set to 1 |
| FILE | compulsory | none | file on which to output the effective energy drift |
| PRINT_STRIDE | compulsory | none | frequency to which output the effective energy drift on FILE |
| ENSEMBLE | optional | false |  Set to TRUE if you want to average over multiple replicas |
| FMT | optional | not used | the format that should be used to output real numbers |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

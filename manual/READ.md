# Action: READ

| Description    | Usage |
|:--------|:--------:|
| Read quantities from a colvar file. | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=READ)[![used in 17 eggs](https://img.shields.io/badge/nest-17-green.svg)](https://www.plumed-nest.org/browse.html?search=READ) | 

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
| STRIDE | compulsory | none |  the frequency with which the file should be read |
| EVERY | compulsory | none |  only read every nth line of the colvar file |
| VALUES | compulsory | none | the values to read from the file |
| FILE | compulsory | none | the name of the file from which to read these quantities |
| IGNORE_TIME | optional | false |  ignore the time in the colvar file |
| IGNORE_FORCES | optional | false |  use this flag if the forces added by any bias can be safely ignored |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

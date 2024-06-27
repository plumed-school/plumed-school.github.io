# Action: PRINT

| Description    | Usage |
|:--------:|:--------:|
| Print quantities to a file. | [![used in 13 tutorials](https://img.shields.io/badge/tutorials-13-green.svg)](https://plumed-school.github.io/browse.html?search=PRINT)[![used in 265 eggs](https://img.shields.io/badge/nest-265-green.svg)](https://www.plumed-nest.org/browse.html?search=PRINT) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| STRIDE | compulsory | none |  the frequency with which the quantities of interest should be output |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |
| FILE | optional | not used | the name of the file on which to output these quantities |
| FMT | optional | not used | the format that should be used to output real numbers |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

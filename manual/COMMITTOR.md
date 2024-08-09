# Action: COMMITTOR

| Description    | Usage |
|:--------|:--------:|
| Does a committor analysis. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=COMMITTOR)[![used in 21 eggs](https://img.shields.io/badge/nest-21-green.svg)](https://www.plumed-nest.org/browse.html?search=COMMITTOR) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| BASIN_LL | compulsory | none | List of lower limits for basin # |
| BASIN_UL | compulsory | none | List of upper limits for basin # |
| STRIDE | compulsory | none |  the frequency with which the CVs are analyzed |
| FILE | optional | not used | the name of the file on which to output the reached basin |
| FMT | optional | not used | the format that should be used to output real numbers |
| NOSTOP | optional | false |  if true do not stop the simulation when reaching a basin but just keep track of it |

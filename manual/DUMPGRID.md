# Action: DUMPGRID

| Description    | Usage |
|:--------|:--------:|
| Output the function on the grid to a file with the PLUMED grid format. | [![used in 6 tutorials](https://img.shields.io/badge/tutorials-6-green.svg)](https://www.plumed-tutorials.org/browse.html?search=DUMPGRID)[![used in 32 eggs](https://img.shields.io/badge/nest-32-green.svg)](https://www.plumed-nest.org/browse.html?search=DUMPGRID) | 

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
| STRIDE | compulsory | none |  the frequency with which the grid should be output to the file |
| FILE | compulsory | none |  the file on which to write the grid |
| GRID | optional | not used | the grid you would like to print (can also use ARG for specifying what is being printed) |
| FMT | optional | not used | the format that should be used to output real numbers |
| PRINT_XYZ | optional | false |  output coordinates on fibonacci grid to xyz file |
| PRINT_ONE_FILE | optional | false |  output grids one after the other in a single file |

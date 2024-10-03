# [Action](actions.md): DUMPCUBE

| Description    | Usage |
|:--------|:--------:|
| Output a three dimensional grid using the Gaussian cube file format. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | grid | the label for the grid that you would like to output |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label for the grid that you would like to output |
| STRIDE | compulsory | 0 |  the frequency with which the grid should be output to the file |
| FILE | compulsory | density |  the file on which to write the grid |
| GRID | optional | not used | the grid you would like to print (can also use ARG for specifying what is being printed) |
| FMT | optional | not used | the format that should be used to output real numbers |
| PRINT_XYZ | optional | false |  output coordinates on fibonacci grid to xyz file |
| PRINT_ONE_FILE | optional | false |  output grids one after the other in a single file |

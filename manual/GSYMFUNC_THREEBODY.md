# [Action](actions.md): GSYMFUNC_THREEBODY

| Description    | Usage |
|:--------|:--------:|
| Calculate functions of the coordinates of the coordinates of all pairs of bonds in the first coordination sphere of an atom | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=GSYMFUNC_THREEBODY)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | matrix | three matrices containing the bond vectors of interest |
| WEIGHT | matrix | the matrix that contains the weights that should be used for each connection |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | three matrices containing the bond vectors of interest |
| WEIGHT | input | none | the matrix that contains the weights that should be used for each connection |
| SERIAL | optional | false |  do the calculation in serial |
| FUNCTION | optional | not used | the parameters of the function you would like to compute |

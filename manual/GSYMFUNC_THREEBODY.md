# Action: GSYMFUNC_THREEBODY

| Description    | Usage |
|:--------|:--------:|
| Calculate functions of the coordinates of the coordinates of all pairs of bonds in the first coordination sphere of an atom | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=GSYMFUNC_THREEBODY)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

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
| WEIGHT | compulsory | none | the matrix that contains the weights that should be used for each connection |
| SERIAL | optional | false |  do the calculation in serial |
| FUNCTION | optional | not used | the parameters of the function you would like to compute |

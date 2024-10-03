# [Shortcut](shortcuts.md): COLLECT_FRAMES

| Description    | Usage |
|:--------|:--------:|
| This allows you to convert a trajectory and a dissimilarity matrix into a dissimilarity object | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=COLLECT_FRAMES)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=COLLECT_FRAMES) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| data | matrix | the data that is being collected by this action | 
| logweights | vector | the logarithms of the weights of the data points | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector | the labels of the values whose time series you would like to collect for later analysis |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the values whose time series you would like to collect for later analysis |
| STRIDE | compulsory | 1 |  the frequency with which data should be stored for analysis |
| CLEAR | compulsory | 0 |  the frequency with which data should all be deleted and restarted |
| ALIGN | compulsory | OPTIMAL |  if storing atoms how would you like the alignment to be done can be SIMPLE/OPTIMAL |
| ATOMS | optional | not used | list of atomic positions that you would like to collect and store for later analysis |
| LOGWEIGHTS | optional | not used | list of actions that calculates log weights that should be used to weight configurations when calculating averages |

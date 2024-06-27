# Action: COLLECT_FRAMES

| Description    | Usage |
|:--------:|:--------:|
| This allows you to convert a trajectory and a dissimilarity matrix into a dissimilarity object | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://plumed-school.github.io/browse.html?search=COLLECT_FRAMES)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=COLLECT_FRAMES) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the arguments you would like to collect |
| STRIDE | compulsory | none |  the frequency with which data should be stored for analysis |
| CLEAR | compulsory | none |  the frequency with which data should all be deleted and restarted |
| ALIGN | compulsory | none |  if storing atoms how would you like the alignment to be done can be SIMPLE/OPTIMAL |
| ARG | optional | not used | the arguments you would like to collect |
| ATOMS | optional | not used | list of atomic positions that you would like to collect and store for later analysis |
| LOGWEIGHTS | optional | not used | list of actions that calculates log weights that should be used to weight configurations when calculating averages |

# Action: LANDMARK_SELECT_FPS

| Description    | Usage |
|:--------:|:--------:|
| Select a of landmarks from a large set of configurations using farthest point sampling. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://plumed-school.github.io/browse.html?search=LANDMARK_SELECT_FPS)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=LANDMARK_SELECT_FPS) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the COLLECT_FRAMES action that you used to get the data |
| NLANDMARKS | compulsory | none | the numbe rof landmarks you would like to create |
| ARG | optional | not used | the COLLECT_FRAMES action that you used to get the data |
| DISSIMILARITIES | optional | not used | the matrix of dissimilarities if this is not provided the squared dissimilarities are calculated |
| SEED | optional | not used | a random number seed |
| NOVORONOI | optional | false |  do not do a Voronoi analysis of the data to determine weights of final points |
| NODISSIMILARITIES | optional | false |  do not calculate the dissimilarities |

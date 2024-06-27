# Action: LANDMARK_SELECT_RANDOM

| Description    | Usage |
|:--------:|:--------:|
| Select a random set of landmarks from a large set of configurations. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

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

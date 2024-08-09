# Action: LANDMARK_SELECT_FPS

| Description    | Usage |
|:--------|:--------:|
| Select a of landmarks from a large set of configurations using farthest point sampling. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=LANDMARK_SELECT_FPS)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=LANDMARK_SELECT_FPS) | 

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| data | scalar | ARG | the data that is being collected by this action | 
| logweights | scalar | ARG | the logarithms of the weights of the data points | 
| rectdissims | scalar | DISSIMILARITIES | a rectangular matrix containing the distances between the landmark points and the rest of the points | 
| sqrdissims | scalar | DISSIMILARITIES | a square matrix containing the distances between each pair of landmark points | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the COLLECT_FRAMES action that you used to get the data |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the COLLECT_FRAMES action that you used to get the data |
| NLANDMARKS | compulsory | none | the numbe rof landmarks you would like to create |
| DISSIMILARITIES | optional | not used | the matrix of dissimilarities if this is not provided the squared dissimilarities are calculated |
| SEED | optional | not used | a random number seed |
| NOVORONOI | optional | false |  do not do a Voronoi analysis of the data to determine weights of final points |
| NODISSIMILARITIES | optional | false |  do not calculate the dissimilarities |

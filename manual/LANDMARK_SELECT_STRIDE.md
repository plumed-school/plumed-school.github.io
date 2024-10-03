# [Shortcut](shortcuts.md): LANDMARK_SELECT_STRIDE

| Description    | Usage |
|:--------|:--------:|
| Select every ith frame from the stored data | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action can calculate the [values](pecifying_arguments.html) in the following table when the associated keyword is included in the input for the action. These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| data | matrix | ARG | the data that is being collected by this action | 
| logweights | vector | ARG | the logarithms of the weights of the data points | 
| rectdissims | matrix | DISSIMILARITIES | a rectangular matrix containing the distances between the landmark points and the rest of the points | 
| sqrdissims | matrix | DISSIMILARITIES | a square matrix containing the distances between each pair of landmark points | 


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| NLANDMARKS | compulsory | none | the numbe rof landmarks you would like to create |
| ARG | optional | not used | the COLLECT_FRAMES action that you used to get the data |
| DISSIMILARITIES | optional | not used | the matrix of dissimilarities if this is not provided the squared dissimilarities are calculated |
| SEED | optional | not used | a random number seed |
| NOVORONOI | optional | false |  do not do a Voronoi analysis of the data to determine weights of final points |
| NODISSIMILARITIES | optional | false |  do not calculate the dissimilarities |

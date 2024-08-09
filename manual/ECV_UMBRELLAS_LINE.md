# Action: ECV_UMBRELLAS_LINE

| Description    | Usage |
|:--------|:--------:|
| Target a multiumbrella ensemble, by combining systems each with a parabolic bias potential at a different location. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=ECV_UMBRELLAS_LINE)[![used in 7 eggs](https://img.shields.io/badge/nest-7-green.svg)](https://www.plumed-nest.org/browse.html?search=ECV_UMBRELLAS_LINE) | 

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
| TEMP | compulsory | none |  temperature |
| CV_MIN | compulsory | none | the minimum of the CV range to be explored |
| CV_MAX | compulsory | none | the maximum of the CV range to be explored |
| SIGMA | compulsory | none | sigma of the umbrella Gaussians |
| SPACING | compulsory | none |  the distance between umbrellas, in units of SIGMA |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| BARRIER | optional | not used | a guess of the free energy barrier to be overcome (better to stay higher than lower) |
| ADD_P0 | optional | false |  add the unbiased Boltzmann distribution to the target distribution, to make sure to sample it |
| LOWER_HALF_ONLY | optional | false |  use only the lower half of each umbrella potentials |

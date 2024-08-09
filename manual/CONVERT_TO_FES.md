# Action: CONVERT_TO_FES

| Description    | Usage |
|:--------|:--------:|
| Convert a histogram to a free energy surface. | [![used in 3 tutorials](https://img.shields.io/badge/tutorials-3-green.svg)](https://www.plumed-tutorials.org/browse.html?search=CONVERT_TO_FES)[![used in 24 eggs](https://img.shields.io/badge/nest-24-green.svg)](https://www.plumed-nest.org/browse.html?search=CONVERT_TO_FES)|
 | **output value** | **type** |
| the free energy surface | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the histogram that you would like to convert into a free energy surface |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the histogram that you would like to convert into a free energy surface |
| GRID | optional | not used | the histogram that you would like to convert into a free energy surface (old syntax) |
| TEMP | optional | not used | the temperature at which you are operating |
| MINTOZERO | optional | false |  set the minimum in the free energy to be equal to zero |

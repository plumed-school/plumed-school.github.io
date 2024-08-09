# Action: BETWEEN

| Description    | Usage |
|:--------|:--------:|
| Use a switching function to determine how many of the input variables are within a certain range. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=BETWEEN)|
 | **output value** | **type** |
| a function that is one if the input falls within a particular range and zero otherwise | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input to this function |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input to this function |
| LOWER | compulsory | none | the lower boundary for this particular bin |
| UPPER | compulsory | none | the upper boundary for this particular bin |
| SMEAR | compulsory | none |  the ammount to smear the Gaussian for each value in the distribution |
| SWITCH | optional | not used | This keyword is used if you want to employ an alternative to the continuous function defined above |

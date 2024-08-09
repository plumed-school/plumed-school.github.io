# Action: STATS

| Description    | Usage |
|:--------|:--------:|
| Calculates statistical properties of a set of collective variables with respect to a set of reference values. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=STATS)[![used in 11 eggs](https://img.shields.io/badge/nest-11-green.svg)](https://www.plumed-nest.org/browse.html?search=STATS) | 

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| sqdevsum | scalar | default | the sum of the squared deviations between arguments and parameters | 
| corr | scalar | default | the correlation between arguments and parameters | 
| slope | scalar | default | the slope of a linear fit between arguments and parameters | 
| intercept | scalar | default | the intercept of a linear fit between arguments and parameters | 
| sqd | scalar | SQDEV | the squared deviations between arguments and parameters | 


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
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| PARARG | optional | not used | the input for this action is the scalar output from one or more other actions without derivatives |
| PARAMETERS | optional | not used | the parameters of the arguments in your function |
| SQDEVSUM | optional | false |  calculates only SQDEVSUM |
| SQDEV | optional | false |  calculates and store the SQDEV as components |
| UPPERDISTS | optional | false |  calculates and store the SQDEV as components |

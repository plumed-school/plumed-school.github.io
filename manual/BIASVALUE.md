# Action: BIASVALUE

| Description    | Usage |
|:--------|:--------:|
| Takes the value of one variable and use it as a bias | [![used in 4 tutorials](https://img.shields.io/badge/tutorials-4-green.svg)](https://www.plumed-tutorials.org/browse.html?search=BIASVALUE)[![used in 52 eggs](https://img.shields.io/badge/nest-52-green.svg)](https://www.plumed-nest.org/browse.html?search=BIASVALUE) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| _bias | scalar | one or multiple instances of this quantity can be referenced elsewhere in the input file | 


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

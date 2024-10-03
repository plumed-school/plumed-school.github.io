# [Action](actions.md): BIASVALUE

| Description    | Usage |
|:--------|:--------:|
| Takes the value of one variable and use it as a bias | [![used in 9 tutorials](https://img.shields.io/badge/tutorials-9-green.svg)](https://www.plumed-tutorials.org/browse.html?search=BIASVALUE)[![used in 52 eggs](https://img.shields.io/badge/nest-52-green.svg)](https://www.plumed-nest.org/browse.html?search=BIASVALUE) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| _bias | scalar | one or multiple instances of this quantity can be referenced elsewhere in the input file | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector | the labels of the scalar/vector arguments whose values will be used as a bias on the system |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the scalar/vector arguments whose values will be used as a bias on the system |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |

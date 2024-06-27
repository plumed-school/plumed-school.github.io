# Action: STATS

| Description    | Usage |
|:--------:|:--------:|
| Calculates statistical properties of a set of collective variables with respect to a set of reference values. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://plumed-school.github.io/browse.html?search=STATS)[![used in 11 eggs](https://img.shields.io/badge/nest-11-green.svg)](https://www.plumed-nest.org/browse.html?search=STATS) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |
| PARARG | optional | not used | the input for this action is the scalar output from one or more other actions without derivatives |
| PARAMETERS | optional | not used | the parameters of the arguments in your function |
| SQDEVSUM | optional | false |  calculates only SQDEVSUM |
| SQDEV | optional | false |  calculates and store the SQDEV as components |
| UPPERDISTS | optional | false |  calculates and store the SQDEV as components |

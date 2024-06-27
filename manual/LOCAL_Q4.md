# Action: LOCAL_Q4

| Description    | Usage |
|:--------:|:--------:|
| Calculate the local degree of order around an atoms by taking the average dot product between the q_4 vector on the central atom and the q_4 vector on the atoms in the first coordination sphere. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=LOCAL_Q4) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| SPECIES | optional | not used |  |
| SPECIESA | optional | not used |  |
| SPECIESB | optional | not used |  |
| SWITCH | optional | not used | This keyword is used if you want to employ an alternative to the continuous swiching function defined above |
| LOWMEM | optional | false |  this flag does nothing and is present only to ensure back-compatibility |
| LESS_THAN | optional | not used | calculate the number of variables that are less than a certain target value |
| MORE_THAN | optional | not used | calculate the number of variables that are more than a certain target value |
| ALT_MIN | optional | not used | calculate the minimum value |
| MIN | optional | not used | calculate the minimum value |
| MAX | optional | not used | calculate the maximum value |
| BETWEEN | optional | not used | calculate the number of values that are within a certain range |
| HIGHEST | optional | false |  this flag allows you to recover the highest of these variables |
| HISTOGRAM | optional | not used | calculate a discretized histogram of the distribution of values |
| LOWEST | optional | false |  this flag allows you to recover the lowest of these variables |
| SUM | optional | false |  calculate the sum of all the quantities |
| MEAN | optional | false |  calculate the mean of all the quantities |

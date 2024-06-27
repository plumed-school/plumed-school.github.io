# Action: CLUSTER_DISTRIBUTION

| Description    | Usage |
|:--------:|:--------:|
| Calculate functions of the distribution of properties in your connected components. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://plumed-school.github.io/browse.html?search=CLUSTER_DISTRIBUTION)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=CLUSTER_DISTRIBUTION) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| CLUSTERS | compulsory | none | the label of the action that does the clustering |
| WEIGHTS | optional | not used | use the vector of values calculated by this action as weights rather than giving each atom a unit weight |
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

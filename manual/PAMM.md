# [Shortcut](shortcuts.md): PAMM

| Description    | Usage |
|:--------|:--------:|
| Probabilistic analysis of molecular motifs. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action can calculate the [values](pecifying_arguments.html) in the following table when the associated keyword is included in the input for the action. These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| lessthan | scalar | LESS_THAN | the number of colvars that have a value less than a threshold | 
| morethan | scalar | MORE_THAN | the number of colvars that have a value more than a threshold | 
| altmin | scalar | ALT_MIN | the minimum value of the cv | 
| min | scalar | MIN | the minimum colvar | 
| max | scalar | MAX | the maximum colvar | 
| between | scalar | BETWEEN | the number of colvars that have a value that lies in a particular interval | 
| highest | scalar | HIGHEST | the largest of the colvars | 
| lowest | scalar | LOWEST | the smallest of the colvars | 
| sum | scalar | SUM | the sum of the colvars | 
| mean | scalar | MEAN | the mean of the colvars | 


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | compulsory | none | the vectors from which the pamm coordinates are calculated |
| CLUSTERS | compulsory | none | the name of the file that contains the definitions of all the clusters |
| REGULARISE | compulsory | 0.001 |  don't allow the denominator to be smaller then this value |
| KERNELS | compulsory | all |  which kernels are we computing the PAMM values for |
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

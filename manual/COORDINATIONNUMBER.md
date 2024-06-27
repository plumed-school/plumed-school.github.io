# Action: COORDINATIONNUMBER

| Description    | Usage |
|:--------:|:--------:|
| Calculate the coordination numbers of atoms so that you can then calculate functions of the distribution of | [![used in 4 tutorials](https://img.shields.io/badge/tutorials-4-green.svg)](https://plumed-school.github.io/browse.html?search=COORDINATIONNUMBER)[![used in 30 eggs](https://img.shields.io/badge/nest-30-green.svg)](https://www.plumed-nest.org/browse.html?search=COORDINATIONNUMBER) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| SPECIES | input | none | this keyword is used for colvars such as coordination number |
| SPECIESA | input | none | this keyword is used for colvars such as the coordination number |
| SPECIESB | input | none | this keyword is used for colvars such as the coordination number |
| NN | compulsory | none |  The n parameter of the switching function  |
| MM | compulsory | none |  The m parameter of the switching function; 0 implies 2*NN |
| D_0 | compulsory | none |  The d_0 parameter of the switching function |
| R_0 | compulsory | none | The r_0 parameter of the switching function |
| R_POWER | compulsory | none | the power to which you want to raise the distance |
| SWITCH | optional | not used | the switching function that it used in the construction of the contact matrix |
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
| LOWMEM | optional | false |  this flag does nothing and is present only to ensure back-compatibility |
| MOMENTS | optional | not used | the list of moments that you would like to calculate |

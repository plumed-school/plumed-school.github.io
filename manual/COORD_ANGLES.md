# Action: COORD_ANGLES

| Description    | Usage |
|:--------:|:--------:|
| Calculate all the angles between bonds in the first coordination spheres of a set of atoms | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=COORD_ANGLES) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| CATOMS | input | none | all the angles between the bonds that radiate out from these central atom are computed |
| GROUP | input | none | a list of angls between pairs of bonds connecting one of the atoms specified using the CATOM command and two of the atoms specified here are computed |
| SWITCH | compulsory | none | the switching function specifies that only those bonds that have a length that is less than a certain threshold are considered |
| LESS_THAN | optional | not used | calculate the number of variables that are less than a certain target value |
| MORE_THAN | optional | not used | calculate the number of variables that are more than a certain target value |
| BETWEEN | optional | not used | calculate the number of values that are within a certain range |
| HISTOGRAM | optional | not used | calculate a discretized histogram of the distribution of values |
| SUM | optional | false |  calculate the sum of all the quantities |
| MEAN | optional | false |  calculate the mean of all the quantities |

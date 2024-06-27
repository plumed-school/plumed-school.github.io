# Action: YDISTANCES

| Description    | Usage |
|:--------:|:--------:|
| Calculate the y components of the vectors connecting one or many pairs of atoms. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| GROUP | input | none | Calculate the distance between each distinct pair of atoms in the group |
| GROUPA | input | none | Calculate the distances between all the atoms in GROUPA and all the atoms in GROUPB |
| GROUPB | input | none | Calculate the distances between all the atoms in GROUPA and all the atoms in GROUPB |
| ATOMS | input | none | the pairs of atoms that you would like to calculate the angles for |
| ORIGIN | input | none | calculate the distance of all the atoms specified using the ATOMS keyword from this point |
| LOCATION | input | none | the location at which the CV is assumed to be in space |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| COMPONENTS | optional | false |  calculate the x, y and z components of the distance separately and store them as label |
| SCALED_COMPONENTS | optional | false |  calculate the a, b and c scaled components of the distance separately and store them as label |
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

# Action: XDISTANCES

| Description    | Usage |
|:--------|:--------:|
| Calculate the x components of the vectors connecting one or many pairs of atoms. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

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
| x | scalar | COMPONENTS | the x-components of the distance vectors | 
| y | scalar | COMPONENTS | the y-components of the distance vectors | 
| z | scalar | COMPONENTS | the z-components of the distance vectors | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| GROUP | atoms | Calculate the distance between each distinct pair of atoms in the group |
| GROUPA | atoms | Calculate the distances between all the atoms in GROUPA and all the atoms in GROUPB |
| GROUPB | atoms | Calculate the distances between all the atoms in GROUPA and all the atoms in GROUPB |
| ATOMS | atoms | the pairs of atoms that you would like to calculate the angles for |
| ORIGIN | atoms | calculate the distance of all the atoms specified using the ATOMS keyword from this point |
| LOCATION | atoms | the location at which the CV is assumed to be in space |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
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

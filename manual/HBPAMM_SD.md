# Action: HBPAMM_SD

| Description    | Usage |
|:--------|:--------:|
| Calculate the number of hydrogen bonds each donor participates in using the HBPamm method | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a matrix containing the weights for the bonds between each pair of atoms | scalar |

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


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the atoms for which you would like to calculate the adjacency matrix |
| GROUPC | atoms |  |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the atoms for which you would like to calculate the adjacency matrix |
| GROUPC | input | none |  |
| NL_CUTOFF | compulsory | none |  The cutoff for the neighbor list |
| NL_STRIDE | compulsory | none |  The frequency with which we are updating the atoms in the neighbor list |
| ORDER | compulsory | none |  the order in which the groups are specified in the input |
| CLUSTERS | compulsory | none | the name of the file that contains the definitions of all the kernels for PAMM |
| REGULARISE | compulsory | none |  don't allow the denominator to be smaller then this value |
| GAUSS_CUTOFF | compulsory | none |  the cutoff at which to stop evaluating the kernel function is set equal to sqrt(2*x)*(max(adc)+cov(adc)) |
| HYDROGENS | compulsory | none | The list of hydrogen atoms that can form part of a hydrogen bond |
| SERIAL | optional | false |  do the calculation in serial |
| NOPBC | optional | false |  don't use pbc |
| SITES | optional | not used | The list of atoms which can be part of a hydrogen bond |
| DONORS | optional | not used | The list of atoms which can donate a hydrogen bond |
| ACCEPTORS | optional | not used | The list of atoms which can accept a hydrogen bond |
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

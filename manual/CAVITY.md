# Action: CAVITY

| Description    | Usage |
|:--------:|:--------:|
| This quantity can be used to calculate functions of the distribution of collective variables for the atoms that lie in a box defined by the positions of four atoms. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ATOMS | input | none | the group of atoms that you would like to investigate |
| BOX | input | none | the positions of four atoms that define spatial extent of the cavity |
| SIGMA | compulsory | none | the width of the function to be used for kernel density estimation |
| KERNEL | compulsory | none |  the type of kernel function to be used |
| SERIAL | optional | false |  do the calculation in serial |
| OUTSIDE | optional | false |  calculate quantities for colvars that are on atoms outside the region of interest |
| PRINT_BOX | optional | false |  write out the positions of the corners of the box to an xyz file |
| FILE | optional | not used | the file on which to write out the box coordinates |
| UNITS | optional | not used |  the units in which to write out the corners of the box |
| DATA | optional | not used | the label of an action that calculates multicolvars |
| LESS_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are less than a certain threshold |
| MORE_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are greater that a certain threshold |
| BETWEEN | optional | not used | calculate the number of colvars that are inside the region of interest and that have a CV value that is between a particular set of bounds |
| SUM | optional | false |  calculate the sum of all the quantities |
| MEAN | optional | false |  calculate the average value of the colvar inside the region of interest |

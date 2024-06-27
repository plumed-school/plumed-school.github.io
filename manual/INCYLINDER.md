# Action: INCYLINDER

| Description    | Usage |
|:--------:|:--------:|
| This quantity can be used to calculate functions of the distribution of collective variables for the atoms that lie in a particular, user-specified part of of the cell. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ATOMS | input | none | the group of atoms that you would like to investigate |
| CENTER | input | none | the atom whose vicinity we are interested in examining |
| KERNEL | compulsory | none |  the type of kernel function to be used |
| DIRECTION | compulsory | none | the direction of the long axis of the cylinder |
| RADIUS | compulsory | none | a switching function that gives the extent of the cylinder in the plane perpendicular to the direction |
| LOWER | compulsory | none |  the lower boundary on the direction parallel to the long axis of the cylinder |
| UPPER | compulsory | none |  the upper boundary on the direction parallel to the long axis of the cylinder |
| SERIAL | optional | false |  do the calculation in serial |
| SIGMA | optional | not used | the width of the function to be used for kernel density estimation |
| OUTSIDE | optional | false |  calculate quantities for colvars that are on atoms outside the region of interest |
| DATA | optional | not used | the label of an action that calculates multicolvars |
| LESS_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are less than a certain threshold |
| MORE_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are greater that a certain threshold |
| BETWEEN | optional | not used | calculate the number of colvars that are inside the region of interest and that have a CV value that is between a particular set of bounds |
| SUM | optional | false |  calculate the sum of all the quantities |
| MEAN | optional | false |  calculate the average value of the colvar inside the region of interest |

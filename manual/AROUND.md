# Action: AROUND

| Description    | Usage |
|:--------:|:--------:|
| This quantity can be used to calculate functions of the distribution of collective variables for the atoms that lie in a particular, user-specified part of of the cell. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=AROUND) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ATOMS | input | none | the group of atoms that you would like to investigate |
| ORIGIN | input | none | the atom whose vicinity we are interested in examining |
| ATOM | input | none | an alternative to ORIGIN |
| SIGMA | compulsory | none | the width of the function to be used for kernel density estimation |
| KERNEL | compulsory | none |  the type of kernel function to be used |
| XLOWER | compulsory | none |  the lower boundary in x relative to the x coordinate of the atom (0 indicates use full extent of box) |
| XUPPER | compulsory | none |  the upper boundary in x relative to the x coordinate of the atom (0 indicates use full extent of box) |
| YLOWER | compulsory | none |  the lower boundary in y relative to the y coordinate of the atom (0 indicates use full extent of box) |
| YUPPER | compulsory | none |  the upper boundary in y relative to the y coordinate of the atom (0 indicates use full extent of box) |
| ZLOWER | compulsory | none |  the lower boundary in z relative to the z coordinate of the atom (0 indicates use full extent of box) |
| ZUPPER | compulsory | none |  the upper boundary in z relative to the z coordinate of the atom (0 indicates use full extent of box) |
| SERIAL | optional | false |  do the calculation in serial |
| OUTSIDE | optional | false |  calculate quantities for colvars that are on atoms outside the region of interest |
| DATA | optional | not used | the label of an action that calculates multicolvars |
| LESS_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are less than a certain threshold |
| MORE_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are greater that a certain threshold |
| BETWEEN | optional | not used | calculate the number of colvars that are inside the region of interest and that have a CV value that is between a particular set of bounds |
| SUM | optional | false |  calculate the sum of all the quantities |
| MEAN | optional | false |  calculate the average value of the colvar inside the region of interest |

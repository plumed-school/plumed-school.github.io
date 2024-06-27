# Action: INENVELOPE

| Description    | Usage |
|:--------:|:--------:|
| This quantity can be used to calculate functions of the distribution of collective variables for the atoms that lie in a region where the density of a certain type of atom is high. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ATOMS | input | none | the group of atoms that you would like to investigate |
| FIELD_ATOMS | input | none | the atom whose positions we are constructing a field from |
| KERNEL | compulsory | none |  the type of kernel function to be used |
| BANDWIDTH | compulsory | none | the bandwidths for kernel density esimtation |
| CONTOUR | compulsory | none | a switching funciton that tells PLUMED how large the density should be |
| CUTOFF | compulsory | none |  the cutoff at which to stop evaluating the kernel functions is set equal to sqrt(2*x)*bandwidth in each direction where x is this number |
| SERIAL | optional | false |  do the calculation in serial |
| OUTSIDE | optional | false |  calculate quantities for colvars that are on atoms outside the region of interest |
| DATA | optional | not used | the label of an action that calculates multicolvars |
| LESS_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are less than a certain threshold |
| MORE_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are greater that a certain threshold |
| BETWEEN | optional | not used | calculate the number of colvars that are inside the region of interest and that have a CV value that is between a particular set of bounds |
| SUM | optional | false |  calculate the sum of all the quantities |
| MEAN | optional | false |  calculate the average value of the colvar inside the region of interest |

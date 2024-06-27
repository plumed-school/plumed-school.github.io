# Action: HBPAMM_MATRIX

| Description    | Usage |
|:--------:|:--------:|
| Adjacency matrix in which two electronegative atoms are adjacent if they are hydrogen bonded | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| GROUP | input | none | the atoms for which you would like to calculate the adjacency matrix |
| GROUPA | input | none |  |
| GROUPB | input | none |  |
| ATOMS | input | none | the atoms for which you would like to calculate the adjacency matrix |
| GROUPC | input | none |  |
| NL_CUTOFF | compulsory | none |  The cutoff for the neighbor list |
| NL_STRIDE | compulsory | none |  The frequency with which we are updating the atoms in the neighbor list |
| ORDER | compulsory | none |  the order in which the groups are specified in the input |
| CLUSTERS | compulsory | none | the name of the file that contains the definitions of all the kernels for PAMM |
| REGULARISE | compulsory | none |  don't allow the denominator to be smaller then this value |
| GAUSS_CUTOFF | compulsory | none |  the cutoff at which to stop evaluating the kernel function is set equal to sqrt(2*x)*(max(adc)+cov(adc)) |
| SERIAL | optional | false |  do the calculation in serial |
| COMPONENTS | optional | false |  also calculate the components of the vector connecting the atoms in the contact matrix |
| NOPBC | optional | false |  don't use pbc |

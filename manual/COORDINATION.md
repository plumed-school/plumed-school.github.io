# Action: COORDINATION

| Description    | Usage |
|:--------:|:--------:|
| Calculate coordination numbers. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://plumed-school.github.io/browse.html?search=COORDINATION)[![used in 54 eggs](https://img.shields.io/badge/nest-54-green.svg)](https://www.plumed-nest.org/browse.html?search=COORDINATION) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| GROUPA | input | none | First list of atoms |
| GROUPB | input | none | Second list of atoms (if empty, N*(N-1)/2 pairs in GROUPA are counted) |
| NN | compulsory | none |  The n parameter of the switching function  |
| MM | compulsory | none |  The m parameter of the switching function; 0 implies 2*NN |
| D_0 | compulsory | none |  The d_0 parameter of the switching function |
| R_0 | compulsory | none | The r_0 parameter of the switching function |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SERIAL | optional | false |  Perform the calculation in serial - for debug purpose |
| PAIR | optional | false |  Pair only 1st element of the 1st group with 1st element in the second, etc |
| NLIST | optional | false |  Use a neighbor list to speed up the calculation |
| NL_CUTOFF | optional | not used | The cutoff for the neighbor list |
| NL_STRIDE | optional | not used | The frequency with which we are updating the atoms in the neighbor list |
| SWITCH | optional | not used | This keyword is used if you want to employ an alternative to the continuous switching function defined above |

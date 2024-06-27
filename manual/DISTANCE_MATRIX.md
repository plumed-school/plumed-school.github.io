# Action: DISTANCE_MATRIX

| Description    | Usage |
|:--------:|:--------:|
| Calculate a matrix of distances | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://plumed-school.github.io/browse.html?search=DISTANCE_MATRIX)[![used in 8 eggs](https://img.shields.io/badge/nest-8-green.svg)](https://www.plumed-nest.org/browse.html?search=DISTANCE_MATRIX) | 

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
| NL_CUTOFF | compulsory | none |  The cutoff for the neighbor list |
| NL_STRIDE | compulsory | none |  The frequency with which we are updating the atoms in the neighbor list |
| CUTOFF | compulsory | none |  ignore distances that have a value larger than this cutoff |
| SERIAL | optional | false |  do the calculation in serial |
| COMPONENTS | optional | false |  also calculate the components of the vector connecting the atoms in the contact matrix |
| NOPBC | optional | false |  don't use pbc |

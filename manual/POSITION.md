# Action: POSITION

| Description    | Usage |
|:--------:|:--------:|
| Calculate the components of the position of an atom. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://plumed-school.github.io/browse.html?search=POSITION)[![used in 27 eggs](https://img.shields.io/badge/nest-27-green.svg)](https://www.plumed-nest.org/browse.html?search=POSITION) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ATOM | input | none | the atom number |
| ATOMS | input | none | the atom numbers that you would like to use the positions of |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| WHOLEMOLECULES | optional | false |  if this is a vector of positions do you want to make the positions into a whole before |
| SCALED_COMPONENTS | optional | false |  calculate the a, b and c scaled components of the position separately and store them as label |

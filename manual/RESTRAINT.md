# Action: RESTRAINT

| Description    | Usage |
|:--------:|:--------:|
| Adds harmonic and/or linear restraints on one or more variables. | [![used in 6 tutorials](https://img.shields.io/badge/tutorials-6-green.svg)](https://plumed-school.github.io/browse.html?search=RESTRAINT)[![used in 26 eggs](https://img.shields.io/badge/nest-26-green.svg)](https://www.plumed-nest.org/browse.html?search=RESTRAINT) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the arguments on which the bias is acting |
| SLOPE | compulsory | none |  specifies that the restraint is linear and what the values of the force constants on each of the variables are |
| KAPPA | compulsory | none |  specifies that the restraint is harmonic and what the values of the force constants on each of the variables are |
| AT | compulsory | none | the position of the restraint |
| ARG | optional | not used | the arguments on which the bias is acting |

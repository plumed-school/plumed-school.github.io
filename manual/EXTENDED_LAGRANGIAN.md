# Action: EXTENDED_LAGRANGIAN

| Description    | Usage |
|:--------:|:--------:|
| Add extended Lagrangian. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| KAPPA | compulsory | none | specifies that the restraint is harmonic and what the values of the force constants on each of the variables are |
| TAU | compulsory | none | specifies that the restraint is harmonic and what the values of the force constants on each of the variables are |
| FRICTION | compulsory | none |  add a friction to the variable |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |
| TEMP | optional | not used | the system temperature - needed when FRICTION is present |

# Action: ABMD

| Description    | Usage |
|:--------:|:--------:|
| Adds a ratchet-and-pawl like restraint on one or more variables. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=ABMD) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| TO | compulsory | none | The array of target values |
| KAPPA | compulsory | none | The array of force constants |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |
| MIN | optional | not used | Array of starting values for the bias (set rho_m(t), otherwise it is set using the current value of ARG) |
| NOISE | optional | not used | Array of white noise intensities (add a temperature to the ABMD) |
| SEED | optional | not used | Array of seeds for the white noise (add a temperature to the ABMD) |

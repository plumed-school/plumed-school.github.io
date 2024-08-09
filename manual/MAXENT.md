# Action: MAXENT

| Description    | Usage |
|:--------|:--------:|
| Add a linear biasing potential on one or more variables that satisfies a maximum entropy principle. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=MAXENT) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| force2 | scalar | the instantaneous value of the squared force due to this bias potential | 
| work | scalar | the instantaneous value of the work done by the biasing force | 
| _work | scalar | the instantaneous value of the work done by the biasing force for each argument | 
| _error | scalar | Instantaneous values of the discrepancy between the observable and the restraint center | 
| _coupling | scalar | Instantaneous values of Lagrangian multipliers | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| KAPPA | compulsory | none |  specifies the initial value for the learning rate |
| TAU | compulsory | none | Specify the dumping time for the learning rate |
| TYPE | compulsory | none | specify the restraint type |
| AT | compulsory | none | the position of the restraint |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ERROR_TYPE | optional | not used | specify the prior on the error to use |
| TSTART | optional | not used | time from where to start averaging the Lagrangian multiplier |
| TEND | optional | not used | time in ps where to stop to compute the average of Lagrangian multiplier |
| ALPHA | optional | not used | default=1 |
| SIGMA | optional | not used | The typical errors expected on observable |
| FILE | optional | not used | Lagrangian multipliers output file |
| LEARN_REPLICA | optional | not used | In a multiple replica environment specify which is the reference replica |
| APPLY_WEIGHTS | optional | not used | Vector of weights containing 1 in correspondence of each replica that will receive the Lagrangian multiplier from the current one |
| PACE | optional | not used | the frequency for Lagrangian multipliers update |
| PRINT_STRIDE | optional | not used | stride of Lagrangian multipliers output file |
| FMT | optional | not used | specify format for Lagrangian multipliers files (useful to decrease the number of digits in regtests) |
| REWEIGHT | optional | false |  to be used with plumed driver in order to reweight a trajectory a posteriori |
| NO_BROADCAST | optional | false |  If active will avoid Lagrangian multipliers to be communicated to other replicas |
| TEMP | optional | not used | the system temperature |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |

# Action: FISST

| Description    | Usage |
|:--------:|:--------:|
| Compute and apply the optimal linear force on an observable to enhance sampling of conformational distributions over a range of applied forces. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=FISST) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| PERIOD | compulsory | none | Steps corresponding to the learning rate |
| NINTERPOLATE | compulsory | none | Number of grid points on which to do interpolation |
| MIN_FORCE | compulsory | none | Minimum force (per CV) to use for sampling |
| MAX_FORCE | compulsory | none | Maximum force (per CV) to use for sampling |
| CENTER | compulsory | none |  The CV value at which the applied bias energy will be zero |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |
| RESET_PERIOD | optional | not used | Reset the learning statistics every time this number of steps comes around |
| KBT | optional | not used | The system temperature in units of KB*T |
| INITIAL_WEIGHT_DIST | optional | not used | Starting distribution for the force weights (options: UNIFORM, EXP, GAUSS) |
| INITIAL_WEIGHT_RATE | optional | not used | Rate of decay for exponential and gaussian distributions |
| RESTART_FMT | optional | not used | the format that should be used to output real numbers in FISST restarts |
| OUT_RESTART | optional | not used | Output file for all information needed to continue FISST simulation |
| IN_RESTART | optional | not used | Read this file to continue an FISST simulation |
| OUT_OBSERVABLE | optional | not used | Output file putting weights needed to compute observables at different force values |
| OBSERVABLE_FREQ | optional | not used |  |
| FREEZE | optional | false |  Fix bias weights at current level (only used for restarting) |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |

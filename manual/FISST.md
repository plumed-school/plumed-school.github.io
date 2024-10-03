# [Action](actions.md): FISST

| Description    | Usage |
|:--------|:--------:|
| Compute and apply the optimal linear force on an observable to enhance sampling of conformational distributions over a range of applied forces. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=FISST)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=FISST) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| force2 | scalar | squared value of force from the bias | 
| _fbar | scalar | For each named CV biased, there will be a corresponding output CV_fbar storing the current linear bias prefactor | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of the scalars on which the bias will act |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the scalars on which the bias will act |
| PERIOD | compulsory | none | Steps corresponding to the learning rate |
| NINTERPOLATE | compulsory | none | Number of grid points on which to do interpolation |
| MIN_FORCE | compulsory | none | Minimum force (per CV) to use for sampling |
| MAX_FORCE | compulsory | none | Maximum force (per CV) to use for sampling |
| CENTER | compulsory | 0 |  The CV value at which the applied bias energy will be zero |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
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

# Action: EDS

| Description    | Usage |
|:--------:|:--------:|
| Add a linear bias on a set of observables. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=EDS) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| RANGE | compulsory | none |  The (starting) maximum increase in coupling constant per PERIOD (in k_B T/[BIAS_SCALE unit]) for each CV biased |
| SEED | compulsory | none |  Seed for random order of changing bias |
| INIT | compulsory | none |  Starting value for coupling constant |
| FIXED | compulsory | none |  Fixed target values for coupling constant |
| LM_MIXING | compulsory | none |  Initial mixing parameter when using Levenberg-Marquadt minimization |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |
| CENTER | optional | not used | The desired centers (equilibrium values) which will be sought during the adaptive linear biasing |
| CENTER_ARG | optional | not used | The desired centers (equilibrium values) which will be sought during the adaptive linear biasing |
| PERIOD | optional | not used | Steps over which to adjust bias for adaptive or ramping |
| BIAS_SCALE | optional | not used | A divisor to set the units of the bias |
| TEMP | optional | not used | The system temperature |
| MULTI_PROP | optional | not used | What proportion of dimensions to update at each step |
| VIRIAL | optional | not used | Add an update penalty for having non-zero virial contributions |
| LOGWEIGHTS | optional | not used | Add weights to use for computing statistics |
| LM | optional | false |  Use Levenberg-Marquadt algorithm along with simultaneous keyword |
| RESTART_FMT | optional | not used | the format that should be used to output real numbers in EDS restarts |
| OUT_RESTART | optional | not used | Output file for all information needed to continue EDS simulation |
| IN_RESTART | optional | not used | Read this file to continue an EDS simulation |
| RAMP | optional | false |  Slowly increase bias constant to a fixed value |
| COVAR | optional | false |  Utilize the covariance matrix when updating the bias |
| FREEZE | optional | false |  Fix bias at current level (only used for restarting) |
| MEAN | optional | false |  Instead of using final bias level from restart, use average |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |

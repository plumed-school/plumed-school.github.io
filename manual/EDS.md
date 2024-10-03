# [Action](actions.md): EDS

| Description    | Usage |
|:--------|:--------:|
| Add a linear bias on a set of observables. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=EDS)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=EDS) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| force2 | scalar | squared value of force from the bias | 
| pressure | scalar | If using virial keyword, this is the current sum of virial terms | 
| _coupling | scalar | For each named CV biased, there will be a corresponding output CV_coupling storing the current linear bias prefactor | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of the scalars on which the bias will act |
| CENTER_ARG | scalar | The desired centers (equilibrium values) which will be sought during the adaptive linear biasing |
| LOGWEIGHTS | scalar | Add weights to use for computing statistics |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the scalars on which the bias will act |
| CENTER_ARG | input | none | The desired centers (equilibrium values) which will be sought during the adaptive linear biasing |
| LOGWEIGHTS | input | none | Add weights to use for computing statistics |
| RANGE | compulsory | 25.0 |  The (starting) maximum increase in coupling constant per PERIOD (in k_B T/[BIAS_SCALE unit]) for each CV biased |
| SEED | compulsory | 0 |  Seed for random order of changing bias |
| INIT | compulsory | 0 |  Starting value for coupling constant |
| FIXED | compulsory | 0 |  Fixed target values for coupling constant |
| LM_MIXING | compulsory | 1 |  Initial mixing parameter when using Levenberg-Marquadt minimization |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| CENTER | optional | not used | The desired centers (equilibrium values) which will be sought during the adaptive linear biasing |
| PERIOD | optional | not used | Steps over which to adjust bias for adaptive or ramping |
| BIAS_SCALE | optional | not used | A divisor to set the units of the bias |
| TEMP | optional | not used | The system temperature |
| MULTI_PROP | optional | not used | What proportion of dimensions to update at each step |
| VIRIAL | optional | not used | Add an update penalty for having non-zero virial contributions |
| LM | optional | false |  Use Levenberg-Marquadt algorithm along with simultaneous keyword |
| RESTART_FMT | optional | not used | the format that should be used to output real numbers in EDS restarts |
| OUT_RESTART | optional | not used | Output file for all information needed to continue EDS simulation |
| IN_RESTART | optional | not used | Read this file to continue an EDS simulation |
| RAMP | optional | false |  Slowly increase bias constant to a fixed value |
| COVAR | optional | false |  Utilize the covariance matrix when updating the bias |
| FREEZE | optional | false |  Fix bias at current level (only used for restarting) |
| MEAN | optional | false |  Instead of using final bias level from restart, use average |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |

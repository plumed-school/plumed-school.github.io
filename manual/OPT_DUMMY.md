# [Action](actions.md): OPT_DUMMY

| Description    | Usage |
|:--------|:--------:|
| Dummy optimizer for debugging. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=OPT_DUMMY)|
 | **output value** | **type** |
| a scalar | scalar |

## Output components

This action can calculate the [values](pecifying_arguments.html) in the following table when the associated keyword is included in the input for the action. These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| gradrms | scalar | MONITOR_INSTANTANEOUS_GRADIENT | the root mean square value of the coefficient gradient | 
| gradmax | scalar | MONITOR_INSTANTANEOUS_GRADIENT | the largest absolute value of the coefficient gradient | 
| avergradrms | scalar | MONITOR_AVERAGE_GRADIENT | the root mean square value of the averaged coefficient gradient | 
| avergradmax | scalar | MONITOR_AVERAGE_GRADIENT | the largest absolute value of the averaged coefficient gradient | 


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| BIAS | compulsory | none | the label of the VES bias to be optimized |
| STRIDE | compulsory | none | the frequency of updating the coefficients given in the number of MD steps |
| COEFFS_FILE | compulsory | coeffs.data |  the name of output file for the coefficients |
| COEFFS_OUTPUT | compulsory | 100 |  how often the coefficients should be written to file |
| COEFFS_FMT | optional | not used | specify format for coefficient file(s) (useful for decrease the number of digits in regtests) |
| COEFFS_SET_ID_PREFIX | optional | not used | suffix to add to the filename given in FILE to identify the bias, should only be given if a single filename is given in FILE when optimizing multiple biases |
| INITIAL_COEFFS | optional | not used | the name(s) of file(s) with the initial coefficients |
| MONITOR_INSTANTANEOUS_GRADIENT | optional | false |  if quantities related to the instantaneous gradient should be outputted |
| TARGETDIST_AVERAGES_FILE | optional | not used | the name of output file for the target distribution averages |
| TARGETDIST_AVERAGES_OUTPUT | optional | not used | how often the target distribution averages should be written out to file |
| BIAS_OUTPUT | optional | not used | how often the bias(es) should be written out to file |
| FES_OUTPUT | optional | not used | how often the FES(s) should be written out to file |
| FES_PROJ_OUTPUT | optional | not used | how often the projections of the FES(s) should be written out to file |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |
| MULTIPLE_WALKERS | optional | false |  if optimization is to be performed using multiple walkers connected via MPI |
| MONITOR_AVERAGE_GRADIENT | optional | false |  if the averaged gradient should be monitored and quantities related to it should be outputted |
| MONITOR_AVERAGES_GRADIENT_EXP_DECAY | optional | not used | use an exponentially decaying averaging with a given time constant when monitoring the averaged gradient |
| MONITOR_HESSIAN | optional | false |  also monitor the Hessian |

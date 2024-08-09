# Action: OPT_ROBBINS_MONRO_SGD

| Description    | Usage |
|:--------|:--------:|
| Robbins-Monro stochastic gradient decent. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a scalar | scalar |

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| gradrms | scalar | MONITOR_INSTANTANEOUS_GRADIENT | the root mean square value of the coefficient gradient | 
| gradmax | scalar | MONITOR_INSTANTANEOUS_GRADIENT | the largest absolute value of the coefficient gradient | 
| stepsize | scalar | default | the current value of step size used to update the coefficients | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| BIAS | compulsory | none | the label of the VES bias to be optimized |
| STRIDE | compulsory | none | the frequency of updating the coefficients given in the number of MD steps |
| COEFFS_FILE | compulsory | none |  the name of output file for the coefficients |
| COEFFS_OUTPUT | compulsory | none |  how often the coefficients should be written to file |
| INITIAL_STEPSIZE | compulsory | none | the initial step size used for the optimization |
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
| MASK_FILE | optional | not used | read in a mask file which allows one to employ different step sizes for different coefficients and/or deactivate the optimization of certain coefficients (by putting values of 0 |
| OUTPUT_MASK_FILE | optional | not used | Name of the file to write out the mask resulting from using the MASK_FILE keyword |
| START_OPTIMIZATION_AFRESH | optional | false |  if the iterations should be started afresh when a restart has been triggered by the RESTART keyword or the MD code |
| TARGETDIST_STRIDE | optional | not used | stride for updating a target distribution that is iteratively updated during the optimization |
| TARGETDIST_OUTPUT | optional | not used | how often the dynamic target distribution(s) should be written out to file |
| TARGETDIST_PROJ_OUTPUT | optional | not used | how often the projections of the dynamic target distribution(s) should be written out to file |
| DECAY_CONSTANT | optional | not used | the decay constant used for the step size |

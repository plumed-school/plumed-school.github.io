# Action: OPES_METAD_EXPLORE

| Description    | Usage |
|:--------|:--------:|
| On-the-fly probability enhanced sampling with well-tempered target distribution in exploreation mode. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=OPES_METAD_EXPLORE)[![used in 8 eggs](https://img.shields.io/badge/nest-8-green.svg)](https://www.plumed-nest.org/browse.html?search=OPES_METAD_EXPLORE) | 

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| bias | scalar | default | the instantaneous value of the bias potential | 
| rct | scalar | default | estimate of c(t) | 
| zed | scalar | default | estimate of Z_n | 
| neff | scalar | default | effective sample size | 
| nker | scalar | default | total number of compressed kernels used to represent the bias | 
| work | scalar | CALC_WORK | total accumulated work done by the bias | 
| nlker | scalar | NLIST | number of kernels in the neighbor list | 
| nlsteps | scalar | NLIST | number of steps from last neighbor list update | 


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
| TEMP | compulsory | none |  temperature |
| PACE | compulsory | none | the frequency for kernel deposition |
| SIGMA | compulsory | none |  the initial widths of the kernels, divided by the square root of gamma |
| BARRIER | compulsory | none | the free energy barrier to be overcome |
| COMPRESSION_THRESHOLD | compulsory | none |  merge kernels if closer than this threshold, in units of sigma |
| FILE | compulsory | none |  a file in which the list of all deposited kernels is stored |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ADAPTIVE_SIGMA_STRIDE | optional | not used | number of steps for measuring adaptive sigma |
| SIGMA_MIN | optional | not used | never reduce SIGMA below this value |
| BIASFACTOR | optional | not used | the gamma bias factor used for the well-tempered target distribution |
| EPSILON | optional | not used | the value of the regularization constant for the probability |
| KERNEL_CUTOFF | optional | not used | truncate kernels at this distance, in units of sigma |
| NLIST_PARAMETERS | optional | not used |  the two cutoff parameters for the kernels neighbor list |
| NLIST | optional | false |  use neighbor list for kernels summation, faster but experimental |
| NLIST_PACE_RESET | optional | false |  force the reset of the neighbor list at each PACE |
| FIXED_SIGMA | optional | false |  do not decrease sigma as the simulation proceeds |
| RECURSIVE_MERGE_OFF | optional | false |  do not recursively attempt kernel merging when a new one is added |
| NO_ZED | optional | false |  do not normalize over the explored CV space, Z_n=1 |
| FMT | optional | not used | specify format for KERNELS file |
| STATE_RFILE | optional | not used | read from this file the compressed kernels and all the info needed to RESTART the simulation |
| STATE_WFILE | optional | not used | write to this file the compressed kernels and all the info needed to RESTART the simulation |
| STATE_WSTRIDE | optional | not used | number of MD steps between writing the STATE_WFILE |
| STORE_STATES | optional | false |  append to STATE_WFILE instead of ovewriting it each time |
| EXCLUDED_REGION | optional | not used | kernels are not deposited when the action provided here has a nonzero value, see example above |
| CALC_WORK | optional | false |  calculate the total accumulated work done by the bias since last restart |
| WALKERS_MPI | optional | false |  switch on MPI version of multiple walkers |
| SERIAL | optional | false |  perform calculations in serial |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

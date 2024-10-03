# [Action](actions.md): METAD

| Description    | Usage |
|:--------|:--------:|
| Used to performed metadynamics on one or more collective variables. | [![used in 10 tutorials](https://img.shields.io/badge/tutorials-10-green.svg)](https://www.plumed-tutorials.org/browse.html?search=METAD)[![used in 161 eggs](https://img.shields.io/badge/nest-161-green.svg)](https://www.plumed-nest.org/browse.html?search=METAD) | 

## Output components

This action can calculate the [values](pecifying_arguments.html) in the following table when the associated keyword is included in the input for the action. These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| bias | scalar | default | the instantaneous value of the bias potential | 
| rbias | scalar | CALC_RCT | the instantaneous value of the bias normalized using the c(t) reweighting factor [rbias=bias-rct] | 
| rct | scalar | CALC_RCT | the reweighting factor c(t) | 
| work | scalar | CALC_WORK | accumulator for work | 
| acc | scalar | ACCELERATION | the metadynamics acceleration factor | 
| maxbias | scalar | CALC_MAX_BIAS | the maximum of the metadynamics V(s, t) | 
| transbias | scalar | CALC_TRANSITION_BIAS | the metadynamics transition bias V*(t) | 
| pace | scalar | FREQUENCY_ADAPTIVE | the hill addition frequency when employing frequency adaptive metadynamics | 
| nlker | scalar | NLIST | number of hills in the neighbor list | 
| nlsteps | scalar | NLIST | number of steps from last neighbor list update | 


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
| SIGMA | compulsory | none | the widths of the Gaussian hills |
| PACE | compulsory | none | the frequency for hill addition |
| FILE | compulsory | HILLS |  a file in which the list of added hills is stored |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| HEIGHT | optional | not used | the heights of the Gaussian hills |
| FMT | optional | not used | specify format for HILLS files (useful for decrease the number of digits in regtests) |
| BIASFACTOR | optional | not used | use well tempered metadynamics and use this bias factor |
| CALC_WORK | optional | false |  calculate the total accumulated work done by the bias since last restart |
| RECT | optional | not used | list of bias factors for all the replicas |
| DAMPFACTOR | optional | not used | damp hills with exp(-max(V)/(kT*DAMPFACTOR) |
| TTBIASFACTOR | optional | not used | use transition tempered metadynamics with this bias factor |
| TTBIASTHRESHOLD | optional | not used | use transition tempered metadynamics with this bias threshold |
| TTALPHA | optional | not used | use transition tempered metadynamics with this hill size decay exponent parameter |
| TARGET | optional | not used | target to a predefined distribution |
| TEMP | optional | not used | the system temperature - this is only needed if you are doing well-tempered metadynamics |
| TAU | optional | not used | in well tempered metadynamics, sets height to (k_B Delta T*pace*timestep)/tau |
| CALC_RCT | optional | false |  calculate the c(t) reweighting factor and use that to obtain the normalized bias [rbias=bias-rct] |
| RCT_USTRIDE | optional | not used | the update stride for calculating the c(t) reweighting factor |
| GRID_MIN | optional | not used | the lower bounds for the grid |
| GRID_MAX | optional | not used | the upper bounds for the grid |
| GRID_BIN | optional | not used | the number of bins for the grid |
| GRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with GRID_BIN) |
| GRID_SPARSE | optional | false |  use a sparse grid to store hills |
| GRID_NOSPLINE | optional | false |  don't use spline interpolation with grids |
| GRID_WSTRIDE | optional | not used | write the grid to a file every N steps |
| GRID_WFILE | optional | not used | the file on which to write the grid |
| GRID_RFILE | optional | not used | a grid file from which the bias should be read at the initial step of the simulation |
| STORE_GRIDS | optional | false |  store all the grid files the calculation generates |
| NLIST | optional | false |  Use neighbor list for kernels summation, faster but experimental |
| NLIST_PARAMETERS | optional | not used |  the two cutoff parameters for the Gaussians neighbor list |
| ADAPTIVE | optional | not used | use a geometric (=GEOM) or diffusion (=DIFF) based hills width scheme |
| SIGMA_MAX | optional | not used | the upper bounds for the sigmas (in CV units) when using adaptive hills |
| SIGMA_MIN | optional | not used | the lower bounds for the sigmas (in CV units) when using adaptive hills |
| WALKERS_ID | optional | not used | walker id |
| WALKERS_N | optional | not used | number of walkers |
| WALKERS_DIR | optional | not used | shared directory with the hills files from all the walkers |
| WALKERS_RSTRIDE | optional | not used | stride for reading hills files |
| WALKERS_MPI | optional | false |  Switch on MPI version of multiple walkers - not compatible with WALKERS_* options other than WALKERS_DIR |
| INTERVAL | optional | not used | one dimensional lower and upper limits, outside the limits the system will not feel the biasing force |
| FLYING_GAUSSIAN | optional | false |  Switch on flying Gaussian method, must be used with WALKERS_MPI |
| ACCELERATION | optional | false |  Set to TRUE if you want to compute the metadynamics acceleration factor |
| ACCELERATION_RFILE | optional | not used | a data file from which the acceleration should be read at the initial step of the simulation |
| CALC_MAX_BIAS | optional | false |  Set to TRUE if you want to compute the maximum of the metadynamics V(s, t) |
| CALC_TRANSITION_BIAS | optional | false |  Set to TRUE if you want to compute a metadynamics transition bias V*(t) |
| TRANSITIONWELL | optional | not used | This keyword appears multiple times as TRANSITIONWELL followed by an integer |
| FREQUENCY_ADAPTIVE | optional | false |  Set to TRUE if you want to enable frequency adaptive metadynamics such that the frequency for hill addition to change dynamically based on the acceleration factor |
| FA_UPDATE_FREQUENCY | optional | not used | the frequency for updating the hill addition pace in frequency adaptive metadynamics, by default this is equal to the value given in PACE |
| FA_MAX_PACE | optional | not used | the maximum hill addition frequency allowed in frequency adaptive metadynamics |
| FA_MIN_ACCELERATION | optional | not used | only update the hill addition pace in frequency adaptive metadynamics after reaching the minimum acceleration factor given here |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

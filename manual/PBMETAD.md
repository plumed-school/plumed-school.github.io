# [Action](actions.md): PBMETAD

| Description    | Usage |
|:--------|:--------:|
| Used to performed Parallel Bias metadynamics. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=PBMETAD)[![used in 31 eggs](https://img.shields.io/badge/nest-31-green.svg)](https://www.plumed-nest.org/browse.html?search=PBMETAD) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of the scalars on which the bias will act |
| PF | scalar | specify which CVs belong in a partitioned family |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the scalars on which the bias will act |
| PF | input | none | specify which CVs belong in a partitioned family |
| SIGMA | compulsory | none | the widths of the Gaussian hills |
| PACE | compulsory | none | the frequency for hill addition, one for all biases |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| FILE | optional | not used | files in which the lists of added hills are stored, default names are assigned using arguments if FILE is not found |
| HEIGHT | optional | not used | the height of the Gaussian hills, one for all biases |
| FMT | optional | not used | specify format for HILLS files (useful for decrease the number of digits in regtests) |
| BIASFACTOR | optional | not used | use well tempered metadynamics with this bias factor, one for all biases |
| TEMP | optional | not used | the system temperature - this is only needed if you are doing well-tempered metadynamics |
| TAU | optional | not used | in well tempered metadynamics, sets height to (k_B Delta T*pace*timestep)/tau |
| GRID_MIN | optional | not used | the lower bounds for the grid |
| GRID_MAX | optional | not used | the upper bounds for the grid |
| GRID_BIN | optional | not used | the number of bins for the grid |
| GRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with GRID_BIN) |
| GRID_SPARSE | optional | false |  use a sparse grid to store hills |
| GRID_NOSPLINE | optional | false |  don't use spline interpolation with grids |
| GRID_WSTRIDE | optional | not used | frequency for dumping the grid |
| GRID_WFILES | optional | not used | dump grid for the bias, default names are used if GRID_WSTRIDE is used without GRID_WFILES |
| GRID_RFILES | optional | not used | read grid for the bias |
| ADAPTIVE | optional | not used | use a geometric (=GEOM) or diffusion (=DIFF) based hills width scheme |
| SIGMA_MAX | optional | not used | the upper bounds for the sigmas (in CV units) when using adaptive hills |
| SIGMA_MIN | optional | not used | the lower bounds for the sigmas (in CV units) when using adaptive hills |
| SELECTOR | optional | not used | add forces and do update based on the value of SELECTOR |
| SELECTOR_ID | optional | not used | value of SELECTOR |
| WALKERS_ID | optional | not used | walker id |
| WALKERS_N | optional | not used | number of walkers |
| WALKERS_DIR | optional | not used | shared directory with the hills files from all the walkers |
| WALKERS_RSTRIDE | optional | not used | stride for reading hills files |
| WALKERS_MPI | optional | false |  Switch on MPI version of multiple walkers - not compatible with WALKERS_* options other than WALKERS_DIR |
| INTERVAL_MIN | optional | not used | one dimensional lower limits, outside the limits the system will not feel the biasing force |
| INTERVAL_MAX | optional | not used | one dimensional upper limits, outside the limits the system will not feel the biasing force |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| UPDATE_FROM | optional | not used | Only update this action from this time |
| UPDATE_UNTIL | optional | not used | Only update this action until this time |

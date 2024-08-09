# Action: DRR

| Description    | Usage |
|:--------|:--------:|
| Used to performed extended-system adaptive biasing force(eABF) | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 6 eggs](https://img.shields.io/badge/nest-6-green.svg)](https://www.plumed-nest.org/browse.html?search=DRR) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| _fict | scalar | one or multiple instances of this quantity can be referenced elsewhere in the input file | 
| _vfict | scalar | one or multiple instances of this quantity can be referenced elsewhere in the input file | 
| _biasforce | scalar | The bias force from eABF/DRR of the fictitious particle | 
| _springforce | scalar | Spring force between real CVs and extended CVs | 
| _fictNoPBC | scalar | the positions of fictitious particles (without PBC) | 


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
| TAU | compulsory | none |  specifies relaxation time on each of variables are, similar to extended Time Constant in Colvars |
| FRICTION | compulsory | none |  add a friction to the variable, similar to extended Langevin Damping in Colvars |
| GRID_MIN | compulsory | none | the lower bounds for the grid (GRID_BIN or GRID_SPACING should be specified) |
| GRID_MAX | compulsory | none | the upper bounds for the grid (GRID_BIN or GRID_SPACING should be specified) |
| REFLECTINGWALL | compulsory | none |  whether add reflecting walls for each CV at GRID_MIN and GRID_MAX |
| FULLSAMPLES | compulsory | none |  number of samples in a bin prior to application of the ABF |
| MAXFACTOR | compulsory | none |  maximum scaling factor of biasing force |
| OUTPUTFREQ | compulsory | none | write results to a file every N steps |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| KAPPA | optional | not used | specifies that the restraint is harmonic and what the values of the force constants on each of the variables are (default to k_BT/(GRID_SPACING)^2) |
| GRID_BIN | optional | not used | the number of bins for the grid |
| GRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with GRID_BIN) |
| ZGRID_MIN | optional | not used | the lower bounds for the grid (ZGRID_BIN or ZGRID_SPACING should be specified) |
| ZGRID_MAX | optional | not used | the upper bounds for the grid (ZGRID_BIN or ZGRID_SPACING should be specified) |
| ZGRID_BIN | optional | not used | the number of bins for the grid |
| ZGRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with ZGRID_BIN) |
| EXTERNAL_FORCE | optional | not used | use forces from other action instead of internal spring force, this disable the extended system! |
| EXTERNAL_FICT | optional | not used | position of external fictitious particles, useful for UIESTIMATOR |
| HISTORYFREQ | optional | not used | save history to a file every N steps |
| NOCZAR | optional | false |  disable the CZAR estimator |
| UI | optional | false |  enable the umbrella integration estimator |
| UIRESTARTPREFIX | optional | not used | specify the restart files for umbrella integration |
| OUTPUTPREFIX | optional | not used | specify the output prefix (default to the label name) |
| TEMP | optional | not used | the system temperature - needed when FRICTION is present |
| EXTTEMP | optional | not used | the temperature of extended variables (default to system temperature) |
| DRR_RFILE | optional | not used | specifies the restart file ( |
| NOBIAS | optional | false |  DO NOT apply bias forces |
| TEXTOUTPUT | optional | false |  use text output for grad and count files instead of boost::serialization binary output |
| MERGEHISTORYFILES | optional | false |  output all historic results to a single file rather than multiple  |
| FMT | optional | not used | specify format for outfiles files (useful for decrease the number of digits in regtests) |

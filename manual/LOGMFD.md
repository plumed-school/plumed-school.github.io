# Action: LOGMFD

| Description    | Usage |
|:--------|:--------:|
| Used to perform LogMFD, LogPD, and TAMD/d-AFED. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| _fict | scalar | For example, the fictitious collective variable for LogMFD is specified as ARG=dist12 and LABEL=logmfd in LOGMFD section in Plumed input file, the associated fictitious dynamical variable can be specified as PRINT ARG=dist12,logmfd | 
| _vfict | scalar | For example, the fictitious collective variable for LogMFD is specified as ARG=dist12 and LABEL=logmfd in LOGMFD section in Plumed input file, the velocity of the associated fictitious dynamical variable can be specified as PRINT ARG=dist12,logmfd | 


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
| INTERVAL | compulsory | none | Period of MD steps (N_m) to update fictitious dynamical variables |
| DELTA_T | compulsory | none | Time step for the fictitious dynamical variables (DELTA_T=1 often works) |
| THERMOSTAT | compulsory | none | Type of thermostat for the fictitious dynamical variables |
| KAPPA | compulsory | none | Spring constant of the harmonic restraining potential |
| FICT_MAX | compulsory | none | Maximum values reachable for the fictitious dynamical variables |
| FICT_MIN | compulsory | none | Minimum values reachable for the fictitious dynamical variables |
| FLOG | compulsory | none | The initial free energy value in the LogMFD/PD run |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| TEMP | optional | not used | Target temperature for the fictitious dynamical variables in LogMFD/PD |
| TAMD | optional | not used | When TAMD=1, TAMD/d-AFED calculations can be performed instead of LogMFD |
| ALPHA | optional | not used | Alpha parameter for LogMFD |
| GAMMA | optional | not used | Gamma parameter for LogMFD |
| FICT | optional | not used | The initial values of the fictitious dynamical variables |
| VFICT | optional | not used | The initial velocities of the fictitious dynamical variables |
| MFICT | optional | not used | Masses of each fictitious dynamical variable |
| XETA | optional | not used | The initial eta variable of the Nose-Hoover thermostat for the fictitious dynamical variables |
| VETA | optional | not used | The initial velocity of eta variable |
| META | optional | not used | Mass of eta variable |
| WORK | optional | not used | The initial value of the work done by fictitious dynamical variables in each replica |
| TEMPPD | optional | not used | Temperature of the Boltzmann factor in the Jarzynski weight in LogPD (Gromacs only) |

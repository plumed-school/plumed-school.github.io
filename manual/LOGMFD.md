# Action: LOGMFD

| Description    | Usage |
|:--------:|:--------:|
| Used to perform LogMFD, LogPD, and TAMD/d-AFED. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| INTERVAL | compulsory | none | Period of MD steps (N_m) to update fictitious dynamical variables |
| DELTA_T | compulsory | none | Time step for the fictitious dynamical variables (DELTA_T=1 often works) |
| THERMOSTAT | compulsory | none | Type of thermostat for the fictitious dynamical variables |
| KAPPA | compulsory | none | Spring constant of the harmonic restraining potential |
| FICT_MAX | compulsory | none | Maximum values reachable for the fictitious dynamical variables |
| FICT_MIN | compulsory | none | Minimum values reachable for the fictitious dynamical variables |
| FLOG | compulsory | none | The initial free energy value in the LogMFD/PD run |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |
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

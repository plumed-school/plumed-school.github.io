# Action: RDC

| Description    | Usage |
|:--------|:--------:|
| Calculates the (Residual) Dipolar Coupling between two atoms. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 3 eggs](https://img.shields.io/badge/nest-3-green.svg)](https://www.plumed-nest.org/browse.html?search=RDC) | 

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| score | scalar | default | the Metainference score | 
| sigma | scalar | default | uncertainty parameter | 
| sigmaMean | scalar | default | uncertainty in the mean estimate | 
| neff | scalar | default | effective number of replicas | 
| acceptSigma | scalar | default | MC acceptance for sigma values | 
| acceptScale | scalar | SCALEDATA | MC acceptance for scale value | 
| acceptFT | scalar | GENERIC | MC acceptance for general metainference f tilde value | 
| weight | scalar | REWEIGHT | weights of the weighted average | 
| biasDer | scalar | REWEIGHT | derivatives with respect to the bias | 
| scale | scalar | SCALEDATA | scale parameter | 
| offset | scalar | ADDOFFSET | offset parameter | 
| ftilde | scalar | GENERIC | ensemble average estimator | 
| rdc | scalar | default | the calculated # RDC | 
| exp | scalar | SVD/COUPLING | the experimental # RDC | 
| Sxx | scalar | SVD | Tensor component | 
| Syy | scalar | SVD | Tensor component | 
| Szz | scalar | SVD | Tensor component | 
| Sxy | scalar | SVD | Tensor component | 
| Sxz | scalar | SVD | Tensor component | 
| Syz | scalar | SVD | Tensor component | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |
| ATOMS | atoms | the couple of atoms involved in each of the bonds for which you wish to calculate the RDC |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| ATOMS | input | none | the couple of atoms involved in each of the bonds for which you wish to calculate the RDC |
| NOISETYPE | compulsory | none |  functional form of the noise (GAUSS,MGAUSS,OUTLIERS,MOUTLIERS,GENERIC) |
| LIKELIHOOD | compulsory | none |  the likelihood for the GENERIC metainference model, GAUSS or LOGN |
| DFTILDE | compulsory | none |  fraction of sigma_mean used to evolve ftilde |
| SCALE0 | compulsory | none |  initial value of the scaling factor |
| SCALE_PRIOR | compulsory | none |  either FLAT or GAUSSIAN |
| OFFSET0 | compulsory | none |  initial value of the offset |
| OFFSET_PRIOR | compulsory | none |  either FLAT or GAUSSIAN |
| SIGMA0 | compulsory | none |  initial value of the uncertainty parameter |
| SIGMA_MIN | compulsory | none |  minimum value of the uncertainty parameter |
| SIGMA_MAX | compulsory | none |  maximum value of the uncertainty parameter |
| OPTSIGMAMEAN | compulsory | none |  Set to NONE/SEM to manually set sigma mean, or to estimate it on the fly |
| WRITE_STRIDE | compulsory | none |  write the status to a file every N steps, this can be used for restart/continuation |
| GYROM | compulsory | none |  Add the product of the gyromagnetic constants for the bond |
| SCALE | compulsory | none |  Add the scaling factor to take into account concentration and other effects |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| DOSCORE | optional | false |  activate metainference |
| NOENSEMBLE | optional | false |  don't perform any replica-averaging |
| REWEIGHT | optional | false |  simple REWEIGHT using the ARG as energy |
| AVERAGING | optional | not used | Stride for calculation of averaged weights and sigma_mean |
| SCALEDATA | optional | false |  Set to TRUE if you want to sample a scaling factor common to all values and replicas |
| SCALE_MIN | optional | not used | minimum value of the scaling factor |
| SCALE_MAX | optional | not used | maximum value of the scaling factor |
| DSCALE | optional | not used | maximum MC move of the scaling factor |
| ADDOFFSET | optional | false |  Set to TRUE if you want to sample an offset common to all values and replicas |
| OFFSET_MIN | optional | not used | minimum value of the offset |
| OFFSET_MAX | optional | not used | maximum value of the offset |
| DOFFSET | optional | not used | maximum MC move of the offset |
| REGRES_ZERO | optional | not used | stride for regression with zero offset |
| DSIGMA | optional | not used | maximum MC move of the uncertainty parameter |
| SIGMA_MEAN0 | optional | not used | starting value for the uncertainty in the mean estimate |
| SIGMA_MAX_STEPS | optional | not used | Number of steps used to optimise SIGMA_MAX, before that the SIGMA_MAX value is used |
| TEMP | optional | not used | the system temperature - this is only needed if code doesn't pass the temperature to plumed |
| MC_STEPS | optional | not used | number of MC steps |
| MC_CHUNKSIZE | optional | not used | MC chunksize |
| STATUS_FILE | optional | not used | write a file with all the data useful for restart/continuation of Metainference |
| SELECTOR | optional | not used | name of selector |
| NSELECT | optional | not used | range of values for selector [0, N-1] |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SVD | optional | false |  Set to TRUE if you want to back calculate using Single Value Decomposition (need GSL at compilation time) |
| COUPLING | optional | not used | Add an experimental value for each coupling (needed by SVD and useful for STATS) |

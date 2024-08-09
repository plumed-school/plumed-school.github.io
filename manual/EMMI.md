# Action: EMMI

| Description    | Usage |
|:--------|:--------:|
| Calculate the fit of a structure or ensemble of structures with a cryo-EM density map. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 6 eggs](https://img.shields.io/badge/nest-6-green.svg)](https://www.plumed-nest.org/browse.html?search=EMMI) | 

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| scoreb | scalar | default | Bayesian score | 
| acc | scalar | NOISETYPE | MC acceptance for uncertainty | 
| scale | scalar | REGRESSION | scale factor | 
| accscale | scalar | REGRESSION | MC acceptance for scale regression | 
| enescale | scalar | REGRESSION | MC energy for scale regression | 
| anneal | scalar | ANNEAL | annealing factor | 
| weight | scalar | REWEIGHT | weights of the weighted average | 
| biasDer | scalar | REWEIGHT | derivatives with respect to the bias | 
| sigma | scalar | NOISETYPE | uncertainty in the forward models and experiment | 
| neff | scalar | default | effective number of replicas | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |
| ATOMS | atoms | atoms for which we calculate the density map, typically all heavy atoms |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| ATOMS | input | none | atoms for which we calculate the density map, typically all heavy atoms |
| GMM_FILE | compulsory | none | file with the parameters of the GMM components |
| NL_CUTOFF | compulsory | none | The cutoff in overlap for the neighbor list |
| NL_STRIDE | compulsory | none | The frequency with which we are updating the neighbor list |
| SIGMA_MIN | compulsory | none | minimum uncertainty |
| RESOLUTION | compulsory | none | Cryo-EM map resolution |
| NOISETYPE | compulsory | none | functional form of the noise (GAUSS, OUTLIERS, MARGINAL) |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SIGMA0 | optional | not used | initial value of the uncertainty |
| DSIGMA | optional | not used | MC step for uncertainties |
| MC_STRIDE | optional | not used | Monte Carlo stride |
| ERR_FILE | optional | not used | file with experimental or GMM fit errors |
| OV_FILE | optional | not used | file with experimental overlaps |
| NORM_DENSITY | optional | not used | integral of the experimental density |
| STATUS_FILE | optional | not used | write a file with all the data useful for restart |
| WRITE_STRIDE | optional | not used | write the status to a file every N steps, this can be used for restart |
| REGRESSION | optional | not used | regression stride |
| REG_SCALE_MIN | optional | not used | regression minimum scale |
| REG_SCALE_MAX | optional | not used | regression maximum scale |
| REG_DSCALE | optional | not used | regression maximum scale MC move |
| SCALE | optional | not used | scale factor |
| ANNEAL | optional | not used | Length of annealing cycle |
| ANNEAL_FACT | optional | not used | Annealing temperature factor |
| TEMP | optional | not used | temperature |
| PRIOR | optional | not used | exponent of uncertainty prior |
| WRITE_OV_STRIDE | optional | not used | write model overlaps every N steps |
| WRITE_OV | optional | not used | write a file with model overlaps |
| AVERAGING | optional | not used | Averaging window for weights |
| NO_AVER | optional | false |  don't do ensemble averaging in multi-replica mode |
| REWEIGHT | optional | false |  simple REWEIGHT using the ARG as energy |

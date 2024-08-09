# Action: VES_DELTA_F

| Description    | Usage |
|:--------|:--------:|
| Implementation of VES Delta F method | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=VES_DELTA_F) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| rct | scalar | the reweighting factor c(t) | 
| work | scalar | the work done by the bias in one AV_STRIDE | 


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
| FILE_F | compulsory | none | names of files containing local free energies and derivatives |
| BIASFACTOR | compulsory | none |  the gamma bias factor used for well-tempered target p(s) |
| M_STEP | compulsory | none |  the mu step used for the Omega functional minimization |
| AV_STRIDE | compulsory | none |  number of simulation steps between alpha updates |
| ALPHA_FILE | compulsory | none |  file name for output minimization parameters |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| TEMP | optional | not used | temperature is compulsory, but it can be sometimes fetched from the MD engine |
| NORMALIZE | optional | false |  normalize all local free energies so that alpha will be (approx) Delta F |
| NO_MINTOZERO | optional | false |  leave local free energies as provided, without shifting them to zero min |
| TG_STRIDE | optional | not used |  number of AV_STRIDE between updates of target p(s) and reweighing factor c(t) |
| TAU_MEAN | optional | not used | exponentially decaying average for alpha (rescaled using AV_STRIDE) |
| INITIAL_ALPHA | optional | not used |  an initial guess for the bias potential parameter alpha |
| DAMPING_OFF | optional | false |  do not use an AdaGrad-like term to rescale M_STEP |
| PRINT_STRIDE | optional | not used |  stride for printing to ALPHA_FILE |
| FMT | optional | not used | specify format for ALPHA_FILE |
| SERIAL | optional | false |  perform the calculation in serial even if multiple tasks are available |
| MULTIPLE_WALKERS | optional | false |  use multiple walkers connected via MPI for the optimization |
| RESTART | optional | not used | allows per-action setting of restart (YES/NO/AUTO) |

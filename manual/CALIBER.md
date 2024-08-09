# Action: CALIBER

| Description    | Usage |
|:--------|:--------:|
| Add a time-dependent, harmonic restraint on one or more variables. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| bias | scalar | default | the instantaneous value of the bias potential | 
| x0 | scalar | default | the instantaneous value of the center of the potential | 
| mean | scalar | default | the current average value of the calculated observable | 
| kappa | scalar | default | the current force constant | 
| scale | scalar | REGRES_ZERO | the current scaling constant | 


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
| FILE | compulsory | none | the name of the file containing the time-resolved values |
| KAPPA | compulsory | none | a force constant, this can be use to scale a constant estimated on-the-fly using AVERAGING |
| TSCALE | compulsory | none |  Apply a time scaling on the experimental time scale |
| SCALE | compulsory | none |  Apply a constant scaling on the data provided as arguments |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOENSEMBLE | optional | false |  don't perform any replica-averaging |
| AVERAGING | optional | not used | Stride for calculation of the optimum kappa, if 0 only KAPPA is used |
| REGRES_ZERO | optional | not used | stride for regression with zero offset |

# Action: ABMD

| Description    | Usage |
|:--------|:--------:|
| Adds a ratchet-and-pawl like restraint on one or more variables. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| force2 | scalar | the instantaneous value of the squared force due to this bias potential | 
| _min | scalar | one or multiple instances of this quantity can be referenced elsewhere in the input file | 


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
| TO | compulsory | none | The array of target values |
| KAPPA | compulsory | none | The array of force constants |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| MIN | optional | not used | Array of starting values for the bias (set rho_m(t), otherwise it is set using the current value of ARG) |
| NOISE | optional | not used | Array of white noise intensities (add a temperature to the ABMD) |
| SEED | optional | not used | Array of seeds for the white noise (add a temperature to the ABMD) |

# [Action](actions.md): VES_LINEAR_EXPANSION

| Description    | Usage |
|:--------|:--------:|
| Linear basis set expansion bias. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=VES_LINEAR_EXPANSION)[![used in 12 eggs](https://img.shields.io/badge/nest-12-green.svg)](https://www.plumed-nest.org/browse.html?search=VES_LINEAR_EXPANSION) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| force2 | scalar | the instantaneous value of the squared force due to this bias potential | 


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
| BASIS_FUNCTIONS | compulsory | none | the label of the one dimensional basis functions that should be used |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| TEMP | optional | not used | the system temperature - this is needed if the MD code does not pass the temperature to PLUMED |
| BIAS_FILE | optional | not used | filename of the file on which the bias should be written out |
| FES_FILE | optional | not used | filename of the file on which the FES should be written out |
| TARGETDIST_FILE | optional | not used | filename of the file on which the target distribution should be written out |
| OPTIMIZATION_THRESHOLD | optional | not used | Threshold value to turn off optimization of localized basis functions |
| COEFFS | optional | not used | read in the coefficients from files |
| TARGET_DISTRIBUTION | optional | not used | the label of the target distribution to be used |
| BIAS_CUTOFF | optional | not used | cutoff the bias such that it only fills the free energy surface up to certain level F_cutoff, here you should give the value of the F_cutoff |
| BIAS_CUTOFF_FERMI_LAMBDA | optional | not used | the lambda value used in the Fermi switching function for the bias cutoff (BIAS_CUTOFF), the default value is 10 |
| GRID_BINS | optional | not used | the number of bins used for the grid |
| PROJ_ARG | optional | not used | arguments for doing projections of the FES or the target distribution |

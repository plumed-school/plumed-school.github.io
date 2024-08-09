# Action: TD_MULTICANONICAL

| Description    | Usage |
|:--------|:--------:|
| Multicanonical target distribution (dynamic). | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=TD_MULTICANONICAL) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| THRESHOLD | compulsory | none |  Maximum exploration free energy in kT |
| EPSILON | compulsory | none |  The zeros of the target distribution are changed to e^-EPSILON |
| MIN_TEMP | compulsory | none | Minimum temperature |
| MAX_TEMP | compulsory | none | Maximum temperature |
| STEPS_TEMP | optional | not used | Number of temperature steps |
| SIGMA | optional | not used | The standard deviation parameters of the Gaussian kernels used for smoothing the target distribution |

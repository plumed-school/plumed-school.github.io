# [Action](actions.md): TD_MULTITHERMAL_MULTIBARIC

| Description    | Usage |
|:--------|:--------:|
| Multithermal-multibaric target distribution (dynamic). | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=TD_MULTITHERMAL_MULTIBARIC) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| THRESHOLD | compulsory | 5 |  Maximum exploration free energy in kT |
| EPSILON | compulsory | 10 |  The zeros of the target distribution are changed to e^-EPSILON |
| MIN_TEMP | compulsory | none | Minimum energy |
| MAX_TEMP | compulsory | none | Maximum energy |
| MIN_PRESSURE | compulsory | none | Minimum pressure |
| MAX_PRESSURE | compulsory | none | Maximum pressure |
| PRESSURE | compulsory | none | Target pressure of the barostat used in the MD engine |
| STEPS_TEMP | compulsory | 20 |  Number of temperature steps |
| STEPS_PRESSURE | compulsory | 20 |  Number of pressure steps |
| SIGMA | optional | not used | The standard deviation parameters of the Gaussian kernels used for smoothing the target distribution |

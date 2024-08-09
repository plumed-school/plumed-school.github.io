# Action: ENSEMBLE

| Description    | Usage |
|:--------|:--------:|
| Calculates the replica averaging of a collective variable over multiple replicas. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=ENSEMBLE)[![used in 9 eggs](https://img.shields.io/badge/nest-9-green.svg)](https://www.plumed-nest.org/browse.html?search=ENSEMBLE) | 

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
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| REWEIGHT | optional | false |  simple REWEIGHT using the latest ARG as energy |
| CENTRAL | optional | false |  calculate a central moment instead of a standard moment |
| TEMP | optional | not used | the system temperature - this is only needed if you are reweighting |
| MOMENT | optional | not used | the moment you want to calculate in alternative to the mean or the variance |
| POWER | optional | not used | the power of the mean (and moment) |

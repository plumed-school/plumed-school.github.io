# [Action](actions.md): RESCALE

| Description    | Usage |
|:--------|:--------:|
| Scales the value of an another action, being a Collective Variable or a Bias. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| igamma | scalar | gamma parameter | 
| accgamma | scalar | MC acceptance for gamma | 
| wtbias | scalar | well-tempered bias | 


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
| TEMP | compulsory | none | temperature |
| SELECTOR | compulsory | none | name of the SELECTOR used for rescaling |
| MAX_RESCALE | compulsory | none | maximum values for rescaling |
| NBIN | compulsory | none | number of bins for gamma grid |
| W0 | compulsory | none | initial bias height |
| BIASFACTOR | compulsory | none | bias factor |
| BSTRIDE | compulsory | none | stride for writing bias |
| BFILE | compulsory | none | file name for bias |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOT_SHARED | optional | not used | list of arguments (from 1 to N) not summed across replicas |
| NOT_RESCALED | optional | not used | these last N arguments will not be scaled |
| MC_STEPS | optional | not used | number of MC steps |
| MC_STRIDE | optional | not used | MC stride |
| PACE | optional | not used | Pace for adding bias, in MC stride unit |

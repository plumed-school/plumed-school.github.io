# [Action](actions.md): EXTENDED_LAGRANGIAN

| Description    | Usage |
|:--------|:--------:|
| Add extended Lagrangian. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=EXTENDED_LAGRANGIAN)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| _fict | scalar | one or multiple instances of this quantity can be referenced elsewhere in the input file | 
| _vfict | scalar | one or multiple instances of this quantity can be referenced elsewhere in the input file | 


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
| KAPPA | compulsory | none | specifies that the restraint is harmonic and what the values of the force constants on each of the variables are |
| TAU | compulsory | none | specifies that the restraint is harmonic and what the values of the force constants on each of the variables are |
| FRICTION | compulsory | 0.0 |  add a friction to the variable |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| TEMP | optional | not used | the system temperature - needed when FRICTION is present |

# Action: MOVINGRESTRAINT

| Description    | Usage |
|:--------|:--------:|
| Add a time-dependent, harmonic restraint on one or more variables. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 10 eggs](https://img.shields.io/badge/nest-10-green.svg)](https://www.plumed-nest.org/browse.html?search=MOVINGRESTRAINT) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| work | scalar | the total work performed changing this restraint | 
| force2 | scalar | the instantaneous value of the squared force due to this bias potential | 
| _cntr | scalar | one or multiple instances of this quantity can be referenced elsewhere in the input file | 
| _work | scalar | one or multiple instances of this quantity can be referenced elsewhere in the input file | 
| _kappa | scalar | one or multiple instances of this quantity can be referenced elsewhere in the input file | 


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
| VERSE | compulsory | none |  Tells plumed whether the restraint is only acting for CV larger (U) or smaller (L) than the restraint or whether it is acting on both sides (B) |
| STEP | compulsory | none | This keyword appears multiple times as STEPx with x=0,1,2, |
| AT | compulsory | none | ATx is equal to the position of the restraint at time STEPx |
| KAPPA | compulsory | none | KAPPAx is equal to the value of the force constants at time STEPx |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |

# Action: RESTRAINT

| Description    | Usage |
|:--------|:--------:|
| Adds harmonic and/or linear restraints on one or more variables. | [![used in 6 tutorials](https://img.shields.io/badge/tutorials-6-green.svg)](https://www.plumed-tutorials.org/browse.html?search=RESTRAINT)[![used in 27 eggs](https://img.shields.io/badge/nest-27-green.svg)](https://www.plumed-nest.org/browse.html?search=RESTRAINT) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| force2 | scalar | the instantaneous value of the squared force due to this bias potential | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the arguments on which the bias is acting |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the arguments on which the bias is acting |
| SLOPE | compulsory | none |  specifies that the restraint is linear and what the values of the force constants on each of the variables are |
| KAPPA | compulsory | none |  specifies that the restraint is harmonic and what the values of the force constants on each of the variables are |
| AT | compulsory | none | the position of the restraint |

# Action: PATHMSD

| Description    | Usage |
|:--------|:--------:|
| This Colvar calculates path collective variables. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 11 eggs](https://img.shields.io/badge/nest-11-green.svg)](https://www.plumed-nest.org/browse.html?search=PATHMSD) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| sss | scalar | the position on the path | 
| zzz | scalar | the distance from the path | 


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
| LAMBDA | compulsory | none | the lambda parameter is needed for smoothing, is in the units of plumed |
| REFERENCE | compulsory | none | the pdb is needed to provide the various milestones |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| NEIGH_SIZE | optional | not used | size of the neighbor list |
| NEIGH_STRIDE | optional | not used | how often the neighbor list needs to be calculated in time units |
| EPSILON | optional | not used |  the maximum distance between the close and the current structure, the positive value turn on the close structure method |
| LOG_CLOSE | optional | not used |  value 1 enables logging regarding the close structure |
| DEBUG_CLOSE | optional | not used |  value 1 enables extensive debugging info regarding the close structure, the simulation will run much slower |

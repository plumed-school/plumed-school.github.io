# Action: FUNCPATHGENERAL

| Description    | Usage |
|:--------|:--------:|
| This function calculates path collective variables (PCVs) using an arbitrary combination of collective variables. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=FUNCPATHGENERAL) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| s | scalar | Position on the path | 
| z | scalar | Distance from the path | 


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
| LAMBDA | compulsory | none | Lambda parameter required for smoothing |
| COEFFICIENTS | compulsory | none | Coefficients to be assigned to the CVs |
| REFERENCE | compulsory | none | Colvar file needed to provide the CV milestones |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| COLUMNS | optional | not used | List of columns in the reference colvar file specifying the CVs |
| NEIGH_SIZE | optional | not used | Size of the neighbor list |
| NEIGH_STRIDE | optional | not used | How often the neighbor list needs to be calculated in time units |

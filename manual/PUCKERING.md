# Action: PUCKERING

| Description    | Usage |
|:--------|:--------:|
|  Calculate sugar pseudorotation coordinates. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 3 eggs](https://img.shields.io/badge/nest-3-green.svg)](https://www.plumed-nest.org/browse.html?search=PUCKERING) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| phs | scalar | Pseudorotation phase (5 membered rings) | 
| amp | scalar | Pseudorotation amplitude (5 membered rings) | 
| Zx | scalar | Pseudorotation x Cartesian component (5 membered rings) | 
| Zy | scalar | Pseudorotation y Cartesian component (5 membered rings) | 
| phi | scalar | Pseudorotation phase (6 membered rings) | 
| theta | scalar | Theta angle (6 membered rings) | 
| amplitude | scalar | Pseudorotation amplitude (6 membered rings) | 
| qx | scalar | Cartesian component x (6 membered rings) | 
| qy | scalar | Cartesian component y (6 membered rings) | 
| qz | scalar | Cartesian component z (6 membered rings) | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the five or six atoms of the sugar ring in the proper order |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the five or six atoms of the sugar ring in the proper order |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |

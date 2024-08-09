# Action: POSITION

| Description    | Usage |
|:--------|:--------:|
| Calculate the components of the position of an atom. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=POSITION)[![used in 27 eggs](https://img.shields.io/badge/nest-27-green.svg)](https://www.plumed-nest.org/browse.html?search=POSITION) | 

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| x | scalar | default | the x-component of the atom position | 
| y | scalar | default | the y-component of the atom position | 
| z | scalar | default | the z-component of the atom position | 
| a | scalar | SCALED_COMPONENTS | the normalized projection on the first lattice vector of the atom position | 
| b | scalar | SCALED_COMPONENTS | the normalized projection on the second lattice vector of the atom position | 
| c | scalar | SCALED_COMPONENTS | the normalized projection on the third lattice vector of the atom position | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOM | atoms | the atom number |
| ATOMS | atoms | the atom numbers that you would like to use the positions of |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOM | input | none | the atom number |
| ATOMS | input | none | the atom numbers that you would like to use the positions of |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| WHOLEMOLECULES | optional | false |  if this is a vector of positions do you want to make the positions into a whole before |
| SCALED_COMPONENTS | optional | false |  calculate the a, b and c scaled components of the position separately and store them as label |

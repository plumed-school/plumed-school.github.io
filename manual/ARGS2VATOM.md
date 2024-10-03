# [Action](actions.md): ARGS2VATOM

| Description    | Usage |
|:--------|:--------:|
| Create a virtual atom from the input scalars | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=ARGS2VATOM) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| x | scalar | the x coordinate of the virtual atom | 
| y | scalar | the y coordinate of the virtual atom | 
| z | scalar | the z coordinate of the virtual atom | 
| mass | scalar | the mass of the virtual atom | 
| charge | scalar | the charge of the virtual atom | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| XPOS | scalar | the value to use for the x position of the atom |
| YPOS | scalar | the value to use for the y position of the atom |
| ZPOS | scalar | the value to use for the z position of the atom |
| MASS | scalar | the value to use for the mass of the atom |
| CHARGE | scalar | the value to use for the charge of the atom |
| XBKP | scalar | x position to use in case PBC not set when using PHASES |
| YBKP | scalar | y position to use in case PBC not set when using PHASES |
| ZBKP | scalar | z position to use in case PBC not set when using PHASES |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| XPOS | input | none | the value to use for the x position of the atom |
| YPOS | input | none | the value to use for the y position of the atom |
| ZPOS | input | none | the value to use for the z position of the atom |
| MASS | input | none | the value to use for the mass of the atom |
| CHARGE | input | none | the value to use for the charge of the atom |
| XBKP | input | none | x position to use in case PBC not set when using PHASES |
| YBKP | input | none | y position to use in case PBC not set when using PHASES |
| ZBKP | input | none | z position to use in case PBC not set when using PHASES |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| FRACTIONAL | optional | false |  the input arguments are calculated in fractional coordinates so you need to multiply by the cell |

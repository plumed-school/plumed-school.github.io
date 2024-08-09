# Action: ARGS2VATOM

| Description    | Usage |
|:--------|:--------:|
| Create a virtual atom from the input scalars | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=ARGS2VATOM) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| x | scalar | the x coordinate of the virtual atom | 
| y | scalar | the y coordinate of the virtual atom | 
| z | scalar | the z coordinate of the virtual atom | 
| mass | scalar | the mass of the virtual atom | 
| charge | scalar | the charge of the virtual atom | 


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
| XPOS | compulsory | none | the x position of the atom |
| YPOS | compulsory | none | the y position of the atom |
| ZPOS | compulsory | none | the z position of the atom |
| MASS | compulsory | none | the mass of the atom |
| CHARGE | compulsory | none | the charge of the atom |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| FRACTIONAL | optional | false |  the input arguments are calculated in fractional coordinates so you need to multiply by the cell |

# Action: PLANE

| Description    | Usage |
|:--------|:--------:|
| Calculate the plane perpendicular to two vectors in order to represent the orientation of a planar molecule. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| x | scalar | the x-component of the vector that is normal to the plane containing the atoms | 
| y | scalar | the y-component of the vector that is normal to the plane containing the atoms | 
| z | scalar | the z-component of the vector that is normal to the plane containing the atoms | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the three or four atoms whose plane we are computing |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the three or four atoms whose plane we are computing |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |

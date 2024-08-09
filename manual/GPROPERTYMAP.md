# Action: GPROPERTYMAP

| Description    | Usage |
|:--------|:--------:|
| Property maps but with a more flexible framework for the distance metric being used. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| gspath | scalar | GPATH | the position along the path calculated using the geometric formula | 
| gzpath | scalar | GPATH | the distance from the path calculated using the geometric formula | 
| spath | scalar | default | the position along the path calculated | 
| zpath | scalar | default | the distance from the path calculated | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the list of arguments you would like to use in your definition of the path |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the list of arguments you would like to use in your definition of the path |
| REFERENCE | compulsory | none | a pdb file containing the set of reference configurations |
| TYPE | compulsory | none |  the manner in which distances are calculated |
| LAMBDA | compulsory | none | the lambda parameter is needed for smoothing, is in the units of plumed |
| COEFFICIENTS | optional | not used | the coefficients of the displacements along each argument that should be used when calculating the euclidean distance |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| NOSPATH | optional | false |  do not calculate the spath CV |
| NOZPATH | optional | false |  do not calculate the zpath CV |
| GPATH | optional | false |  calculate the trigonometric path |
| PROPERTY | optional | not used | the property to be used in the index |

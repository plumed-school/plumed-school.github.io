# Action: GPATH

| Description    | Usage |
|:--------|:--------:|
| Distance along and from a path calculated using geometric formulas | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=GPATH)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=GPATH) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| s | scalar | the position on the path | 
| z | scalar | the distance from the path | 


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
| COEFFICIENTS | optional | not used | the coefficients of the displacements along each argument that should be used when calculating the euclidean distance |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| NOSPATH | optional | false |  do not calculate the spath CV |
| NOZPATH | optional | false |  do not calculate the zpath CV |
| GPATH | optional | false |  calculate the trigonometric path |
| PROPERTY | optional | not used | read in path coordinates by finding option with this label in remark of pdb frames |

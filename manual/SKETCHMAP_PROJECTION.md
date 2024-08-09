# Action: SKETCHMAP_PROJECTION

| Description    | Usage |
|:--------|:--------:|
| Read in a sketch-map projection | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=SKETCHMAP_PROJECTION)|
 | **output value** | **type** |
| the out-of-sample projections of the input arguments using the input sketch-map projection | scalar |

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
| PROPERTY | compulsory | none | the property to be used in the index |
| WEIGHT | compulsory | none | the weight of each individual landmark in the stress fucntion that is to be optimised |
| HIGH_DIM_FUNCTION | compulsory | none | the parameters of the switching function in the high dimensional space |
| LOW_DIM_FUNCTION | compulsory | none | the parameters of the switching function in the low dimensional space |
| CGTOL | compulsory | none |  The tolerance for the conjugate gradient minimization that finds the out of sample projections |
| COEFFICIENTS | optional | not used | the coefficients of the displacements along each argument that should be used when calculating the euclidean distance |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| NOSPATH | optional | false |  do not calculate the spath CV |
| NOZPATH | optional | false |  do not calculate the zpath CV |
| GPATH | optional | false |  calculate the trigonometric path |

# Action: ADAPTIVE_PATH

| Description    | Usage |
|:--------|:--------:|
| Compute path collective variables that adapt to the lowest free energy path connecting states A and B. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the position along and from the adaptive path | scalar |

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
| FIXED | compulsory | none | the positions in the list of input frames of the two path nodes whose positions remain fixed during the path optimization |
| HALFLIFE | compulsory | none |  the number of MD steps after which a previously measured path distance weighs only 50 percent in the average |
| UPDATE | compulsory | none | the frequency with which the path should be updated |
| TOLERANCE | compulsory | none |  the tolerance to use for the path updating algorithm that makes all frames equidistant |
| FMT | compulsory | none |  the format to use for output files |
| WSTRIDE | compulsory | none | frequency with which to write out the path |
| COEFFICIENTS | optional | not used | the coefficients of the displacements along each argument that should be used when calculating the euclidean distance |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| NOSPATH | optional | false |  do not calculate the spath CV |
| NOZPATH | optional | false |  do not calculate the zpath CV |
| GPATH | optional | false |  calculate the trigonometric path |
| PROPERTY | optional | not used | read in path coordinates by finding option with this label in remark of pdb frames |
| WFILE | optional | not used | file on which to write out the path |

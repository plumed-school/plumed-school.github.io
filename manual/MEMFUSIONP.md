# Action: MEMFUSIONP

| Description    | Usage |
|:--------|:--------:|
| Calculate a CV that can induce the formation of the hemifusion stalk between two initially flat and planar bilayers. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the value of the CV | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| UMEMBRANE | atoms | all the beads of the upper membrane |
| LMEMBRANE | atoms | all the beads of the lower membrane |
| TAILS | atoms | all the tail beads of the system |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| UMEMBRANE | input | none | all the beads of the upper membrane |
| LMEMBRANE | input | none | all the beads of the lower membrane |
| TAILS | input | none | all the tail beads of the system |
| NSMEM | compulsory | none | the number of slices of the membrane fusion cylinder in such a way that when the bilayers are flat and parallel the CV is equal to 0 |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| DSMEM | optional | not used |  thickness of the slices of the membrane fusion cylinder |
| HMEM | optional | not used |  parameter of the step function θ(x,h) for the membrane fusion |
| RCYLMEM | optional | not used |  the radius of the membrane fusion cylinder |
| ZETAMEM | optional | not used |  occupation factor |
| ONEOVERS2C2CUTOFF | optional | not used |  cut off large values for the derivative of the atan2 function |
| XCYL | optional | not used | X coordinate of the fixed cylinder, if not present this will be calculated |
| YCYL | optional | not used | Y coordinate of the fixed cylinder, if not present this will be calculated |

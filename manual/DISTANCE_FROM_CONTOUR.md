# Action: DISTANCE_FROM_CONTOUR

| Description    | Usage |
|:--------:|:--------:|
| Calculate the perpendicular distance from a Willard-Chandler dividing surface. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=DISTANCE_FROM_CONTOUR) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| POSITIONS | input | none | the positions of the atoms that we are calculating the contour from |
| ATOM | input | none | The atom whose perpendicular distance we are calculating from the contour |
| BANDWIDTH | compulsory | none | the bandwidths for kernel density esimtation |
| KERNEL | compulsory | none |  the kernel function you are using |
| CUTOFF | compulsory | none |  the cutoff at which to stop evaluating the kernel functions is set equal to sqrt(2*x)*bandwidth in each direction where x is this number |
| CONTOUR | compulsory | none | the value we would like for the contour |
| DIR | compulsory | none | the direction perpendicular to the contour that you are looking for |
| TOLERANCE | compulsory | none |  this parameter is used to manage periodic boundary conditions |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |

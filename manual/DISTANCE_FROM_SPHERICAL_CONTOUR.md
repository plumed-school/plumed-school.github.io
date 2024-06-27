# Action: DISTANCE_FROM_SPHERICAL_CONTOUR

| Description    | Usage |
|:--------:|:--------:|
| Calculate the perpendicular distance from a Willard-Chandler dividing surface. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| POSITIONS | input | none | the positions of the atoms that we are calculating the contour from |
| ATOM | input | none | The atom whose perpendicular distance we are calculating from the contour |
| ORIGIN | input | none | The position of the center of the region that the contour encloses |
| BANDWIDTH | compulsory | none | the bandwidths for kernel density esimtation |
| KERNEL | compulsory | none |  the kernel function you are using |
| CUTOFF | compulsory | none |  the cutoff at which to stop evaluating the kernel functions is set equal to sqrt(2*x)*bandwidth in each direction where x is this number |
| CONTOUR | compulsory | none | the value we would like for the contour |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |

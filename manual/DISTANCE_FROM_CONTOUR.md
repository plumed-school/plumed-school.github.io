# Action: DISTANCE_FROM_CONTOUR

| Description    | Usage |
|:--------|:--------:|
| Calculate the perpendicular distance from a Willard-Chandler dividing surface. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=DISTANCE_FROM_CONTOUR) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| dist1 | scalar | the distance between the reference atom and the nearest contour | 
| dist2 | scalar | the distance between the reference atom and the other contour | 
| qdist | scalar | the differentiable (squared) distance between the two contours (see above) | 
| thickness | scalar | the distance between the two contours on the line from the reference atom | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |
| POSITIONS | atoms | the positions of the atoms that we are calculating the contour from |
| ATOM | atoms | The atom whose perpendicular distance we are calculating from the contour |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| POSITIONS | input | none | the positions of the atoms that we are calculating the contour from |
| ATOM | input | none | The atom whose perpendicular distance we are calculating from the contour |
| BANDWIDTH | compulsory | none | the bandwidths for kernel density esimtation |
| KERNEL | compulsory | none |  the kernel function you are using |
| CUTOFF | compulsory | none |  the cutoff at which to stop evaluating the kernel functions is set equal to sqrt(2*x)*bandwidth in each direction where x is this number |
| CONTOUR | compulsory | none | the value we would like for the contour |
| DIR | compulsory | none | the direction perpendicular to the contour that you are looking for |
| TOLERANCE | compulsory | none |  this parameter is used to manage periodic boundary conditions |

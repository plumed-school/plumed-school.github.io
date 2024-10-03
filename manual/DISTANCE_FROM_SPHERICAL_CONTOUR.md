# [Action](actions.md): DISTANCE_FROM_SPHERICAL_CONTOUR

| Description    | Usage |
|:--------|:--------:|
| Calculate the perpendicular distance from a Willard-Chandler dividing surface. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| dist | scalar | the distance between the reference atom and the nearest contour | 
| radius | scalar | the radial distance from the center of the contour to the edge | 


## Input

The [arguments](specifying_arguments.html) and [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | vector | the label of the weights to use when constructing the density |
| POSITIONS | atoms | the positions of the atoms that we are calculating the contour from |
| ATOM | atoms | The atom whose perpendicular distance we are calculating from the contour |
| ORIGIN | atoms | The position of the center of the region that the contour encloses |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the label of the weights to use when constructing the density |
| POSITIONS | input | none | the positions of the atoms that we are calculating the contour from |
| ATOM | input | none | The atom whose perpendicular distance we are calculating from the contour |
| ORIGIN | input | none | The position of the center of the region that the contour encloses |
| BANDWIDTH | compulsory | none | the bandwidths for kernel density esimtation |
| KERNEL | compulsory | GAUSSIAN |  the kernel function you are using |
| CUTOFF | compulsory | 6.25 |  the cutoff at which to stop evaluating the kernel functions is set equal to sqrt(2*x)*bandwidth in each direction where x is this number |
| CONTOUR | compulsory | none | the value we would like for the contour |

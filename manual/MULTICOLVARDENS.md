# [Shortcut](shortcuts.md): MULTICOLVARDENS

| Description    | Usage |
|:--------|:--------:|
| Evaluate the average value of a multicolvar on a grid. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=MULTICOLVARDENS)|
 | **output value** | **type** |
| the average value of the order parameters at each point on the grid | grid |

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| STRIDE | compulsory | 1 |  the frequency with which to accumulate the densities |
| CLEAR | compulsory | 0 |  the frequency with which to clear the density |
| ORIGIN | compulsory | none | we will use the position of this atom as the origin |
| DIR | compulsory | none | the direction in which to calculate the density profile |
| KERNEL | compulsory | GAUSSIAN |  the kernel function you are using |
| BANDWIDTH | optional | not used | the bandwidths for kernel density esimtation |
| NBINS | optional | not used | the number of bins to use in each direction (alternative to GRID_NBIN) |
| GRID_MIN | optional | not used | the lower bounds for the grid (default boxlengths) |
| GRID_MAX | optional | not used | the upper bounds for the grid (default boxlengths) |
| DATA | optional | not used | the multicolvar which you would like to calculate the density profile for |
| ATOMS | optional | not used | if you are calculating a atomic density you use this keyword to specify the atoms that are involved |
| UNORMALIZED | optional | false |  do not divide by the density |
| NORMALIZATION | optional | not used | set true/false to determine how to the data is normalised |

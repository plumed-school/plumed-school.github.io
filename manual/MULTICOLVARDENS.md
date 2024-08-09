# Action: MULTICOLVARDENS

| Description    | Usage |
|:--------|:--------:|
| Evaluate the average value of a multicolvar on a grid. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=MULTICOLVARDENS)|
 | **output value** | **type** |
| the average value of the order parameters at each point on the grid | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| STRIDE | compulsory | none |  the frequency with which to accumulate the densities |
| CLEAR | compulsory | none |  the frequency with which to clear the density |
| ORIGIN | compulsory | none | we will use the position of this atom as the origin |
| DIR | compulsory | none | the direction in which to calculate the density profile |
| KERNEL | compulsory | none |  the kernel function you are using |
| BANDWIDTH | optional | not used | the bandwidths for kernel density esimtation |
| NBINS | optional | not used | the number of bins to use in each direction (alternative to GRID_NBIN) |
| DATA | optional | not used | the multicolvar which you would like to calculate the density profile for |
| ATOMS | optional | not used | if you are calculating a atomic density you use this keyword to specify the atoms that are involved |
| UNORMALIZED | optional | false |  do not divide by the density |
| NORMALIZATION | optional | not used | set true/false to determine how to the data is normalised |

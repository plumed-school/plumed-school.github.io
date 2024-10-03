# [Shortcut](shortcuts.md): PCA

| Description    | Usage |
|:--------|:--------:|
| Perform principal component analysis (PCA) using either the positions of the atoms a large number of collective variables as input. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=PCA)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the projections of the input coordinates on the PCA components that were found from the covariance matrix | matrix |

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | compulsory | none | the arguments that you would like to make the histogram for |
| NLOW_DIM | compulsory | none | number of low-dimensional coordinates required |
| STRIDE | compulsory | 0 |  the frequency with which to perform this analysis |
| FILE | optional | not used | the file on which to output the low dimensional coordinates |
| FMT | optional | not used | the format to use when outputting the low dimensional coordinates |

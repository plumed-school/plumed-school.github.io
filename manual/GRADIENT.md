# [Shortcut](shortcuts.md): GRADIENT

| Description    | Usage |
|:--------|:--------:|
| Calculate the gradient of an input grid | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the desired gradient | scalar |

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ORIGIN | compulsory | none | we will use the position of this atom as the origin in our calculation |
| NBINS | compulsory | none | number of bins to use in each direction for the calculation of the gradient |
| DIR | compulsory | xyz |  the directions in which we are calculating the graident |
| SIGMA | compulsory | none | the width of the function to be used for kernel density estimation |
| KERNEL | compulsory | gaussian-bin |  the type of kernel function to be used in the grids |
| ATOMS | compulsory | none | calculate the gradient of these atoms |

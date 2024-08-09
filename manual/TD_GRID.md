# Action: TD_GRID

| Description    | Usage |
|:--------|:--------:|
| Target distribution from an external grid file (static). | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=TD_GRID) | 

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
| FILE | compulsory | none | The name of the external grid file to be used as a target distribution |
| SHIFT | optional | not used | Shift the grid read in by some constant value |
| ZERO_OUTSIDE | optional | false |  By default the target distribution is continuous such that values outside the boundary of the external grid file are the same as at the boundary |
| DO_NOT_NORMALIZE | optional | false |  By default the target distribution from the external grid is always normalized inside the code |
| WELLTEMPERED_FACTOR | optional | not used | Broaden the target distribution such that it is taken as [p(s)]^(1/gamma) where gamma is the well tempered factor given here |
| SHIFT_TO_ZERO | optional | false |  Shift the minimum value of the target distribution to zero |

# Action: BF_WAVELETS

| Description    | Usage |
|:--------|:--------:|
| Daubechies Wavelets basis functions. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=BF_WAVELETS) | 

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
| ORDER | compulsory | none | The order of the basis function expansion |
| MINIMUM | compulsory | none | The minimum of the interval on which the basis functions are defined |
| MAXIMUM | compulsory | none | The maximum of the interval on which the basis functions are defined |
| TYPE | compulsory | none | Specify the wavelet type |
| DEBUG_INFO | optional | false |  Print out more detailed information about the basis set |
| FUNCTION_LENGTH | optional | not used | The domain size of the individual basis functions |
| NUM_BF | optional | not used | The number of basis functions that should be used |
| TAILS_THRESHOLD | optional | not used | The threshold for cutting off tail wavelets as a fraction of the maximum value |
| MOTHER_WAVELET | optional | false |  If this flag is set mother wavelets will be used instead of the scaling function (father wavelet) |
| MIN_GRID_SIZE | optional | not used | The minimal number of grid bins of the Wavelet function |
| DUMP_WAVELET_GRID | optional | false |  If this flag is set the grid with the wavelet values will be written to a file |
| WAVELET_FILE_FMT | optional | not used | The number format of the wavelet grid values and derivatives written to file |
| PERIODIC | optional | false |  Use periodic version of basis set |

# Action: WHAM_HISTOGRAM

| Description    | Usage |
|:--------|:--------:|
| This can be used to output the a histogram using the weighted histogram technique | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the histogram that was generated using the WHAM weights | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the arguments that you would like to make the histogram for |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the arguments that you would like to make the histogram for |
| BIAS | compulsory | none |  the value of the biases to use when performing WHAM |
| TEMP | compulsory | none | the temperature at which the simulation was run |
| STRIDE | compulsory | none |  the frequency with which the data should be stored to perform WHAM |
| GRID_MIN | compulsory | none | the minimum to use for the grid |
| GRID_MAX | compulsory | none | the maximum to use for the grid |
| GRID_BIN | compulsory | none | the number of bins to use for the grid |
| BANDWIDTH | optional | not used | the bandwidth for kernel density estimation |

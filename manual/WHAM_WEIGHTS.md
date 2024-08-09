# Action: WHAM_WEIGHTS

| Description    | Usage |
|:--------|:--------:|
| Calculate and output weights for configurations using the weighted histogram analysis method. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the weights that were calculated using WHAM | scalar |

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
| BIAS | compulsory | none |  the value of the biases to use when performing WHAM |
| STRIDE | compulsory | none |  the frequency with which the bias should be stored to perform WHAM |
| FILE | compulsory | none | the file on which to output the WHAM weights |
| TEMP | optional | not used | the temperature at which the simulation was run |
| FMT | optional | not used | the format to use for the real numbers in the output file |

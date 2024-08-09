# Action: KERNEL

| Description    | Usage |
|:--------|:--------:|
| Use a switching function to determine how many of the input variables are less than a certain cutoff. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the value of the kernel evaluated at the argument values | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the arguments that should be used as input to this method |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the arguments that should be used as input to this method |
| TYPE | compulsory | none |  the type of kernel to use |
| CENTER | compulsory | none | the position of the center of the kernel |
| COVAR | compulsory | none | the covariance of the kernel |
| WEIGHT | compulsory | none |  the weight to multiply this kernel function by |
| NUMBER | compulsory | none |  if there are multiple sets of kernel parameters in the input file which set of kernel parameters would you like to read in here |
| SIGMA | optional | not used | square root of variance of the cluster |
| REFERENCE | optional | not used | the file from which to read the kernel parameters |
| NORMALIZED | optional | false |  would you like the kernel function to be normalized |

# Action: VES_OUTPUT_BASISFUNCTIONS

| Description    | Usage |
|:--------|:--------:|
| Output basis functions to file. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=VES_OUTPUT_BASISFUNCTIONS) | 

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
| BASIS_FUNCTIONS | compulsory | none | the label of the basis functions that you want to use |
| GRID_BINS | optional | not used | the number of bins used for the grid for writing the basis function values and derivatives |
| GRID_MIN | optional | not used | the minimum of the grid for writing the basis function values and derivatives |
| GRID_MAX | optional | not used | the maximum of the grid for writing the basis function values and derivatives |
| FILE_VALUES | optional | not used | filename of the file on which the basis function values are written |
| FILE_DERIVS | optional | not used | filename of the file on which the basis function derivatives are written |
| FORMAT_VALUES_DERIVS | optional | not used | the numerical format of the basis function values and derivatives written to file |
| FORMAT_VALUES | optional | not used | the numerical format of the basis function derivatives written to file |
| FORMAT_DERIVS | optional | not used | the numerical format of the basis function values written to file |
| FILE_TARGETDIST_AVERAGES | optional | not used | filename of the file on which the averages over the target distributions are written |
| FORMAT_TARGETDIST_AVERAGES | optional | not used | the numerical format of the target distribution averages written to file |
| FILE_TARGETDIST | optional | not used | filename of the files on which the target distributions are written |
| TARGET_DISTRIBUTION | optional | not used | the target distribution to be used |
| IGNORE_PERIODICITY | optional | false |  if the periodicity of the basis functions should be ignored |
| NUMERICAL_DERIVATIVES | optional | false |  if the derivatives of the basis functions should be calculated numerically |

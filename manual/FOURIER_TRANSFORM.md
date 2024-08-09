# Action: FOURIER_TRANSFORM

| Description    | Usage |
|:--------|:--------:|
| Compute the Discrete Fourier Transform (DFT) by means of FFTW of data stored on a 2D grid. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=FOURIER_TRANSFORM)|
 | **output value** | **type** |
| the fourier transform of the input grid | scalar |

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| real | scalar | FT_TYPE | the real part of the function | 
| imag | scalar | FT_TYPE | the imaginary part of the function | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input for this action is the scalar output from one or more other actions |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| FOURIER_PARAMETERS | compulsory | none |  what kind of normalization is applied to the output and if the Fourier transform in FORWARD or BACKWARD |
| SERIAL | optional | false |  do the calculation in serial |
| FT_TYPE | optional | not used | choose what kind of data you want as output on the grid |

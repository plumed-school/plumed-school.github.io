# Action: FOURIER_TRANSFORM

| Description    | Usage |
|:--------:|:--------:|
| Compute the Discrete Fourier Transform (DFT) by means of FFTW of data stored on a 2D grid. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=FOURIER_TRANSFORM) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| FOURIER_PARAMETERS | compulsory | none |  what kind of normalization is applied to the output and if the Fourier transform in FORWARD or BACKWARD |
| SERIAL | optional | false |  do the calculation in serial |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |
| FT_TYPE | optional | not used | choose what kind of data you want as output on the grid |

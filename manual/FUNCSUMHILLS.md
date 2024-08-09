# Action: FUNCSUMHILLS

| Description    | Usage |
|:--------|:--------:|
| This function is intended to be called by the command line tool sum_hills.  It is meant to integrate a HILLS file or an HILLS file interpreted as a histogram in a variety of ways. It is, therefore, not expected that you use this during your dynamics (it will crash!) | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| a scalar | scalar |

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
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| HILLSFILES | optional | not used |  source file for hills creation(may be the same as HILLS) |
| HISTOFILES | optional | not used |  source file for histogram creation(may be the same as HILLS) |
| HISTOSIGMA | optional | not used |  sigmas for binning when the histogram correction is needed     |
| PROJ | optional | not used |  only with sumhills: the projection on the CVs |
| KT | optional | not used |  only with sumhills: the kt factor when projection on CVs |
| GRID_MIN | optional | not used | the lower bounds for the grid |
| GRID_MAX | optional | not used | the upper bounds for the grid |
| GRID_BIN | optional | not used | the number of bins for the grid |
| GRID_SPACING | optional | not used | the approximate grid spacing (to be used as an alternative or together with GRID_BIN) |
| INTERVAL | optional | not used | set one dimensional INTERVAL |
| OUTHILLS | optional | not used |  output file for hills  |
| OUTHISTO | optional | not used |  output file for histogram  |
| INITSTRIDE | optional | not used |  stride if you want an initial dump  |
| STRIDE | optional | not used |  stride when you do it on the fly  |
| ISCLTOOL | optional | false |  use via plumed command line: calculate at read phase and then go |
| PARALLELREAD | optional | false |  read parallel HILLS file |
| NEGBIAS | optional | false |  dump  negative bias ( -bias )   instead of the free energy: needed in well tempered with flexible hills  |
| NOHISTORY | optional | false |  to be used with INITSTRIDE:  it splits the bias/histogram in pieces without previous history   |
| MINTOZERO | optional | false |  translate the resulting bias/histogram to have the minimum to zero   |
| FMT | optional | not used | the format that should be used to output real numbers |

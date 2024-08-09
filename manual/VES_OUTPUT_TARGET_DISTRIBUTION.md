# Action: VES_OUTPUT_TARGET_DISTRIBUTION

| Description    | Usage |
|:--------|:--------:|
| Output target distribution to file. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

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
| GRID_MIN | compulsory | none | the lower bounds for the grid |
| GRID_MAX | compulsory | none | the upper bounds for the grid |
| GRID_BINS | compulsory | none | the number of bins used for the grid |
| TARGETDIST_FILE | compulsory | none | filename of the file for writing the target distribution |
| TARGET_DISTRIBUTION | compulsory | none | the target distribution to be used |
| GRID_PERIODICITY | optional | not used | specify if the individual arguments should be made periodic (YES) or not (NO) |
| LOG_TARGETDIST_FILE | optional | not used | filename of the file for writing the log of the target distribution |
| FMT_GRIDS | optional | not used | the numerical format of the target distribution grids written to file |
| DO_1D_PROJECTIONS | optional | false |  Also output the one-dimensional marginal distributions for multi-dimensional target distribution |

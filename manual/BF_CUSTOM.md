# Action: BF_CUSTOM

| Description    | Usage |
|:--------|:--------:|
| Basis functions given by arbitrary mathematical expressions. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

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
| MINIMUM | compulsory | none | The minimum of the interval on which the basis functions are defined |
| MAXIMUM | compulsory | none | The maximum of the interval on which the basis functions are defined |
| DEBUG_INFO | optional | false |  Print out more detailed information about the basis set |
| FUNC | optional | not used | The basis functions f_i(x) given in mathematical expressions using _x_ as a variable |
| TRANSFORM | optional | not used | An optional function that can be used to transform the argument before calculating the basis function values |
| PERIODIC | optional | false |  Indicate that the basis functions are periodic |
| CHECK_NAN_INF | optional | false |  Check that the basis functions do not result in a not a number (nan) or infinity (inf) |

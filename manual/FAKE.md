# Action: FAKE

| Description    | Usage |
|:--------|:--------:|
| This is a fake colvar container used by cltools or various other actions that supports input and period definitions | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the fake atom index, a number is enough |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the fake atom index, a number is enough |
| PERIODIC | compulsory | none | if the output of your function is periodic then you should specify the periodicity of the function |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| COMPONENTS | optional | not used | additional components that this variable is supposed to have |

# Action: PYTORCH_MODEL

| Description    | Usage |
|:--------|:--------:|
| Load a PyTorch model compiled with TorchScript. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=PYTORCH_MODEL)[![used in 14 eggs](https://img.shields.io/badge/nest-14-green.svg)](https://www.plumed-nest.org/browse.html?search=PYTORCH_MODEL) | 

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
| FILE | optional | not used | Filename of the PyTorch compiled model |

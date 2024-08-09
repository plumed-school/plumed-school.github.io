# Action: ANN

| Description    | Usage |
|:--------|:--------:|
| Calculates the ANN-function. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=ANN) | 

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
| PERIODIC | compulsory | none | if the output of your function is periodic then you should specify the periodicity of the function |
| NUM_LAYERS | compulsory | none | number of layers of the neural network |
| NUM_NODES | compulsory | none | numbers of nodes in each layer of the neural network |
| ACTIVATIONS | compulsory | none | activation functions for the neural network |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| WEIGHTS | optional | not used | flattened weight arrays connecting adjacent layers, WEIGHTS0 represents flattened weight array connecting layer 0 and layer 1, WEIGHTS1 represents flattened weight array connecting layer 1 and layer 2,  |
| BIASES | optional | not used | bias array for each layer of the neural network, BIASES0 represents bias array for layer 1, BIASES1 represents bias array for layer 2,  |

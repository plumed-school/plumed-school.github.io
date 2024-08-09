# Action: MAZE_OPTIMIZER_BIAS

| Description    | Usage |
|:--------|:--------:|
| Biases the ligand along the direction calculated by the chosen MAZE_OPTIMIZER. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=MAZE_OPTIMIZER_BIAS) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| force2 | scalar | Square of the biasing force | 
| x | scalar | Optimal biasing direction: x component | 
| y | scalar | Optimal biasing direction: y component | 
| z | scalar | Optimal biasing direction: z component | 
| tdist | scalar | Total distance traveled by biased atoms | 


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
| BIASING_RATE | compulsory | none | Biasing rate |
| ALPHA | compulsory | none | Rescaled force constant |
| OPTIMIZER | compulsory | none | Optimization technique to minimize the collective variable for ligand     unbinding: RANDOM_WALK,                STEERED_MD,                RANDOM_ACCELERATION_MD,                SIMULATED_ANNEALING,                MEMETIC_SAMPLING |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |

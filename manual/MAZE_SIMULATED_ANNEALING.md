# [Action](actions.md): MAZE_SIMULATED_ANNEALING

| Description    | Usage |
|:--------|:--------:|
| Calculates the biasing direction along which the ligand unbinds by minimizing | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=MAZE_SIMULATED_ANNEALING) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| x | scalar | Optimal biasing direction; x component | 
| y | scalar | Optimal biasing direction; y component | 
| z | scalar | Optimal biasing direction; z component | 
| loss | scalar | Loss function value defined by the provided pairing function | 
| sr | scalar | Sampling radius | 


## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| LIGAND | atoms | Indices of ligand atoms |
| PROTEIN | atoms | Indices of protein atoms |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| LIGAND | input | none | Indices of ligand atoms |
| PROTEIN | input | none | Indices of protein atoms |
| N_ITER | compulsory | none | Number of optimization steps |
| OPTIMIZER_STRIDE | compulsory | none | Optimizer stride |
| PROBABILITY_DECREASER | compulsory | none | Temperature-like parameter that is decreased during optimization to modify the Metropolis-Hastings acceptance probability |
| COOLING | compulsory | none | Reduction factor for PROBABILITY_DECREASER, should be in (0, 1] |
| COOLING_SCHEME | compulsory | none | Cooling scheme: geometric |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SERIAL | optional | false |  Perform the simulation in serial -- used only for debugging purposes, should not be used otherwise |
| PAIR | optional | false |  Pair only the 1st element of the 1st group with the 1st element in the second, etc |
| NLIST | optional | false |  Use a neighbor list of ligand-protein atom pairs to speed up the calculating of the distances |
| NL_CUTOFF | optional | not used | Neighbor list cut-off for the distances of ligand-protein atom pairs |
| NL_STRIDE | optional | not used | Update stride for the ligand-protein atom pairs in the neighbor list |
| LOSS | optional | not used | Loss function describing ligand-protein interactions required by every optimizer |

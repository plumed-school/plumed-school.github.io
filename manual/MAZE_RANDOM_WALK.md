# Action: MAZE_RANDOM_WALK

| Description    | Usage |
|:--------:|:--------:|
| Fake optimizer that can be used for debugging. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| LIGAND | input | none | Indices of ligand atoms |
| PROTEIN | input | none | Indices of protein atoms |
| OPTIMIZER_STRIDE | compulsory | none | Optimizer stride |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SERIAL | optional | false |  Perform the simulation in serial -- used only for debugging purposes, should not be used otherwise |
| PAIR | optional | false |  Pair only the 1st element of the 1st group with the 1st element in the second, etc |
| NLIST | optional | false |  Use a neighbor list of ligand-protein atom pairs to speed up the calculating of the distances |
| NL_CUTOFF | optional | not used | Neighbor list cut-off for the distances of ligand-protein atom pairs |
| NL_STRIDE | optional | not used | Update stride for the ligand-protein atom pairs in the neighbor list |
| LOSS | optional | not used | Loss function describing ligand-protein interactions required by every optimizer |

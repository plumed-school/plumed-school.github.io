# Action: PLUMED

| Description    | Usage |
|:--------|:--------:|
| Embed a separate PLUMED instance. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

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
| STRIDE | compulsory | none |  stride different from 1 are not supported yet |
| FILE | optional | not used | input file for the guest PLUMED instance |
| KERNEL | optional | not used | kernel to be used for the guest PLUMED instance (USE WITH CAUTION!) |
| LOG | optional | not used | log file for the guest PLUMED instance |
| CHDIR | optional | not used | run guest in a separate directory |
| NOREPLICAS | optional | false |  run multiple replicas as isolated ones, without letting them know that the host has multiple replicas |

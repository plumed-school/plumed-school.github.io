# Action: PCARMSD

| Description    | Usage |
|:--------:|:--------:|
| Calculate the PCA components for a number of provided eigenvectors and an average structure. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| AVERAGE | compulsory | none | a file in pdb format containing the reference structure and the atoms involved in the CV |
| EIGENVECTORS | compulsory | none | a file in pdb format containing the reference structure and the atoms involved in the CV |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SQUARED_ROOT | optional | false |   This should be set if you want RMSD instead of mean squared displacement  |

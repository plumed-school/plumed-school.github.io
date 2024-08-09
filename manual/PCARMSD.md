# Action: PCARMSD

| Description    | Usage |
|:--------|:--------:|
| Calculate the PCA components for a number of provided eigenvectors and an average structure. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| eig | scalar | the projections on each eigenvalue are stored on values labeled eig-1, eig-2,  | 
| residual | scalar | the distance of the present configuration from the configuration supplied as AVERAGE in terms of mean squared displacement after optimal alignment  | 


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
| AVERAGE | compulsory | none | a file in pdb format containing the reference structure and the atoms involved in the CV |
| EIGENVECTORS | compulsory | none | a file in pdb format containing the reference structure and the atoms involved in the CV |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SQUARED_ROOT | optional | false |   This should be set if you want RMSD instead of mean squared displacement  |

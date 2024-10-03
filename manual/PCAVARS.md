# [Shortcut](shortcuts.md): PCAVARS

| Description    | Usage |
|:--------|:--------:|
| Projection on principal component eigenvectors or other high dimensional linear subspace | [![used in 2 tutorials](https://img.shields.io/badge/tutorials-2-green.svg)](https://www.plumed-tutorials.org/browse.html?search=PCAVARS)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=PCAVARS) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| eig | vector | the projections on the eigenvalues | 
| residual | scalar | the residual distance that is not projected on any of the eigenvalues | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector | if there are arguments to be used specify them here |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | if there are arguments to be used specify them here |
| REFERENCE | compulsory | none | a pdb file containing the set of reference configurations |
| TYPE | compulsory | OPTIMAL-FAST |  the manner in which distances are calculated |
| NOPBC | optional | false |  do not use periodic boundary conditions when computing this quantity |

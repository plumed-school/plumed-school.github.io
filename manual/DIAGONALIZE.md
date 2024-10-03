# [Action](actions.md): DIAGONALIZE

| Description    | Usage |
|:--------|:--------:|
| Calculate the eigenvalues and eigenvectors of a square matrix | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=DIAGONALIZE)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| vals | scalar | the eigevalues of the input matrix | 
| vecs | vector | the eigenvectors of the input matrix | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | matrix | the input matrix |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input matrix |
| VECTORS | compulsory | all |  the eigenvalues and vectors that you would like to calculate |
| MATRIX | optional | not used | the input matrix (can use ARG instead) |

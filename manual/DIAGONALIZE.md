# Action: DIAGONALIZE

| Description    | Usage |
|:--------|:--------:|
| Calculate the eigenvalues and eigenvectors of a square matrix | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=DIAGONALIZE)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| vals | scalar | the eigevalues of the input matrix | 
| vecs | scalar | the eigenvectors of the input matrix | 


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
| VECTORS | compulsory | none |  the eigenvalues and vectors that you would like to calculate |
| MATRIX | optional | not used | the input matrix (can use ARG instead) |

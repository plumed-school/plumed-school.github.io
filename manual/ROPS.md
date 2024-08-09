# Action: ROPS

| Description    | Usage |
|:--------|:--------:|
| Calculate the ROPS order parameter | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| the values of the ROPS order parameters | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| SPECIES | atoms | this keyword is used for colvars such as coordination number |
| SPECIESA | atoms | this keyword is used for colvars such as the coordination number |
| SPECIESB | atoms | this keyword is used for colvars such as the coordination number |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| SPECIES | input | none | this keyword is used for colvars such as coordination number |
| SPECIESA | input | none | this keyword is used for colvars such as the coordination number |
| SPECIESB | input | none | this keyword is used for colvars such as the coordination number |
| QUATERNIONS | compulsory | none | the label of the action that computes the quaternions that should be used |
| KERNELFILE_DOPS | compulsory | none | the file containing the list of kernel parameters |
| KERNELFILE_ROPS | compulsory | none | the file containing the list of kernel parameters |
| CUTOFF | compulsory | none | cutoff for the distance matrix |

# [Action](actions.md): METATENSOR

| Description    | Usage |
|:--------|:--------:|
| Use arbitrary machine learning models as collective variables. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| collective variable created by the metatensor model | scalar/vector/matrix |

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| outputs | scalar | collective variable created by the metatensor model | 


## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| SPECIES | atoms | the atoms in each PLUMED species |
| SELECTED_ATOMS | atoms | subset of atoms that should be used for the calculation |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| SPECIES | input | none | the atoms in each PLUMED species |
| SELECTED_ATOMS | input | none | subset of atoms that should be used for the calculation |
| MODEL | compulsory | none | path to the exported metatensor model |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| EXTENSIONS_DIRECTORY | optional | not used | path to the directory containing TorchScript extensions to load |
| DEVICE | optional | not used | Torch device to use for the calculation |
| CHECK_CONSISTENCY | optional | false |  Should we enable internal consistency of the model |
| SPECIES_TO_TYPES | optional | not used | mapping from PLUMED SPECIES to metatensor's atomic types |

# [Shortcut](shortcuts.md): SELECT_COMPONENTS

| Description    | Usage |
|:--------|:--------:|
| Create a new value to hold a subset of the components that are in a vector or matrix | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=SELECT_COMPONENTS)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=SELECT_COMPONENTS)|
 | **output value** | **type** |
| a vector containing the selected components | vector |

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | vector/matrix | the value from which we are selecting components |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the value from which we are selecting components |
| COMPONENTS | compulsory | none | the components in the input value that you woul like to build a new vector from |

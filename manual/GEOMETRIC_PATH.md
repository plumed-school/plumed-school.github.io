# [Action](actions.md): GEOMETRIC_PATH

| Description    | Usage |
|:--------|:--------:|
| Distance along and from a path calculated using geometric formulas | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=GEOMETRIC_PATH)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| s | scalar | the position on the path | 
| z | scalar | the distance from the path | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | matrix | the labels of the matrix that contains the vectors of displacements from each frame in the path |
| REFERENCE | vector | labels for actions that contain reference coordinates for each point on the path |
| PROPERTY | vector | the label of a value that contains the coordinates we are projecting these points onto |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the matrix that contains the vectors of displacements from each frame in the path |
| REFERENCE | input | none | labels for actions that contain reference coordinates for each point on the path |
| PROPERTY | input | none | the label of a value that contains the coordinates we are projecting these points onto |
| METRIC | compulsory | none | the method to use for computing the displacement vectors between the reference frames |
| METRIC_COMPONENT | compulsory | none | if the final action in your metric contains multiple components this keyword is used to specify the component that should be used |
| SERIAL | optional | false |  do the calculation in serial |

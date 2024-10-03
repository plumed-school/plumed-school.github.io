# [Shortcut](shortcuts.md): UPPER_WALLS

| Description    | Usage |
|:--------|:--------:|
| Defines a wall for the value of one or more collective variables, | [![used in 8 tutorials](https://img.shields.io/badge/tutorials-8-green.svg)](https://www.plumed-tutorials.org/browse.html?search=UPPER_WALLS)[![used in 129 eggs](https://img.shields.io/badge/nest-129-green.svg)](https://www.plumed-nest.org/browse.html?search=UPPER_WALLS) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| force2 | scalar | the instantaneous value of the squared force due to this bias potential | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar/vector | the arguments on which the bias is acting |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the arguments on which the bias is acting |
| AT | compulsory | none | the positions of the wall |
| KAPPA | compulsory | none | the force constant for the wall |
| OFFSET | compulsory | 0.0 |  the offset for the start of the wall |
| EXP | compulsory | 2.0 |  the powers for the walls |
| EPS | compulsory | 1.0 |  the values for s_i in the expression for a wall |

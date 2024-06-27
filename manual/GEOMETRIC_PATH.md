# Action: GEOMETRIC_PATH

| Description    | Usage |
|:--------:|:--------:|
| Distance along and from a path calculated using geometric formulas | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://plumed-school.github.io/browse.html?search=GEOMETRIC_PATH)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| ARG | input | none | the input for this action is the scalar output from one or more other actions |
| METRIC | compulsory | none | the method to use for computing the displacement vectors between the reference frames |
| METRIC_COMPONENT | compulsory | none | if the final action in your metric contains multiple components this keyword is used to specify the component that should be used |
| REFERENCE | compulsory | none | labels for actions that contain reference coordinates for each point on the path |
| PROPERTY | compulsory | none | the coordinates we are projecting these points onto |
| SERIAL | optional | false |  do the calculation in serial |
| ARG | optional | not used | the input for this action is the scalar output from one or more other actions |

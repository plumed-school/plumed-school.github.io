# [Action](actions.md): REPARAMETERIZE_PATH

| Description    | Usage |
|:--------|:--------:|
| Take an input path with frames that are not equally spaced and make the frames equally spaced | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | matrix | the labels of the matrix that contains the vectors of displacements from each frame in the path |
| REFERENCE | vector | labels for actions that contain reference coordinates for each point on the path |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the matrix that contains the vectors of displacements from each frame in the path |
| REFERENCE | input | none | labels for actions that contain reference coordinates for each point on the path |
| METRIC | compulsory | none | the method to use for computing the displacement vectors between the reference frames |
| METRIC_COMPONENT | compulsory | none | if the final action in your metric contains multiple components this keyword is used to specify the component that should be used |
| STRIDE | compulsory | 1 |  the frequency with which to reparameterize the path |
| FIXED | compulsory | 0 |  the frames in the path to fix |
| MAXCYLES | compulsory | 100 |  number of cycles of the algorithm to run |
| TOL | compulsory | 1E-4 |  the tolerance to use for the path reparameterization algorithm |
| DISPLACE_FRAMES | optional | not used | label of an action that tells us how to displace the frames |

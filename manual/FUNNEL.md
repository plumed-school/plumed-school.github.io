# [Action](actions.md): FUNNEL

| Description    | Usage |
|:--------|:--------:|
| Calculate a funnel-shape restraint potential that is defined on a grid that is read during the setup. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=FUNNEL) | 

## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the labels of the scalars on which the bias will act |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the scalars on which the bias will act |
| SCALE | compulsory | 1.0 |  a factor that multiplies the external potential, useful to invert free energies |
| MAXS | compulsory | MAXS |  maximum value assumed by fps |
| ZCC | compulsory | ZCC |  switching point between cylinder and cone |
| FILE | compulsory | none | name of the Funnel potential file |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOSPLINE | optional | false |  specifies that no spline interpolation is to be used when calculating the energy and forces due to the external potential |
| SPARSE | optional | false |  specifies that the external potential uses a sparse grid |
| SPHERE | optional | false |  The Funnel potential including the binding site can be spherical instead of a cone |
| NBINS | optional | not used | number of bins along fps |
| NBINZ | optional | not used | number of bins along fps |
| MINS | optional | not used | minimum value assumed by fps |
| KAPPA | optional | not used | constant to be used for the funnel-shape restraint potential |
| RCYL | optional | not used | radius of the cylindrical section |
| SAFETY | optional | not used | To be used in case the SPHERE flag is chosen, it regulates how much the potential extends (in nm) |
| SLOPE | optional | not used | Adjust the behavior of the potential outside the funnel, greater values than 1 |
| ALPHA | optional | not used | angle to change the width of the cone section |
| WALKERS_MPI | optional | false |  To be used when gromacs + multiple walkers are used |

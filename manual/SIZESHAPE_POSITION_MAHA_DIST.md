# Action: SIZESHAPE_POSITION_MAHA_DIST

| Description    | Usage |
|:--------:|:--------:|
| Calculates Mahalanobis distance of a current configuration from a  given reference configurational distribution in size-and-shape space. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| GROUP | input | none | The group of atoms being used |
| PRECISION | compulsory | none | Precision Matrix (inverse of covariance) |
| REFERENCE | compulsory | none | Reference structure |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SQUARED | optional | false |  Returns the square of distance |

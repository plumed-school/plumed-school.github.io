# [Action](actions.md): BF_LEGENDRE

| Description    | Usage |
|:--------|:--------:|
| Legendre polynomials basis functions. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=BF_LEGENDRE)[![used in 8 eggs](https://img.shields.io/badge/nest-8-green.svg)](https://www.plumed-nest.org/browse.html?search=BF_LEGENDRE) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ORDER | compulsory | none | The order of the basis function expansion |
| MINIMUM | compulsory | none | The minimum of the interval on which the basis functions are defined |
| MAXIMUM | compulsory | none | The maximum of the interval on which the basis functions are defined |
| DEBUG_INFO | optional | false |  Print out more detailed information about the basis set |
| NUMERICAL_INTEGRALS | optional | false |  Calculate basis function integral for the uniform distribution numerically |
| SCALED | optional | false |  Scale the polynomials such that they are orthonormal to 1 |

# Action: TD_GENERALIZED_EXTREME_VALUE

| Description    | Usage |
|:--------|:--------:|
| Generalized extreme value distribution (static). | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| LOCATION | compulsory | none | The mu parameter of the generalized extreme value distribution |
| SCALE | compulsory | none | The sigma parameter for the generalized extreme value distribution given as a positive number |
| SHAPE | compulsory | none | The xi parameter for the generalized extreme value distribution |
| WELLTEMPERED_FACTOR | optional | not used | Broaden the target distribution such that it is taken as [p(s)]^(1/gamma) where gamma is the well tempered factor given here |
| SHIFT_TO_ZERO | optional | false |  Shift the minimum value of the target distribution to zero |
| NORMALIZE | optional | false |  Renormalized the target distribution over the intervals on which it is defined to make sure that it is properly normalized to 1 |

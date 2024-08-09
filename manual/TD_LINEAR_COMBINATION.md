# Action: TD_LINEAR_COMBINATION

| Description    | Usage |
|:--------|:--------:|
| Target distribution given by linear combination of distributions (static or dynamic). | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

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
| DISTRIBUTIONS | compulsory | none | The labels of the target distribution actions to be used in the linear combination |
| WEIGHTS | optional | not used | The weights of target distributions |
| WELLTEMPERED_FACTOR | optional | not used | Broaden the target distribution such that it is taken as [p(s)]^(1/gamma) where gamma is the well tempered factor given here |
| NORMALIZE | optional | false |  Renormalized the target distribution over the intervals on which it is defined to make sure that it is properly normalized to 1 |

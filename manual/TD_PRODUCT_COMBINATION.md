# Action: TD_PRODUCT_COMBINATION

| Description    | Usage |
|:--------|:--------:|
| Target distribution given by product combination of distributions (static or dynamic). | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

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
| DISTRIBUTIONS | compulsory | none | The labels of the target distribution actions to be used in the product combination |
| WELLTEMPERED_FACTOR | optional | not used | Broaden the target distribution such that it is taken as [p(s)]^(1/gamma) where gamma is the well tempered factor given here |
| SHIFT_TO_ZERO | optional | false |  Shift the minimum value of the target distribution to zero |

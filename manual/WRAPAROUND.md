# [Action](actions.md): WRAPAROUND

| Description    | Usage |
|:--------|:--------:|
| Rebuild periodic boundary conditions around chosen atoms. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=WRAPAROUND)[![used in 8 eggs](https://img.shields.io/badge/nest-8-green.svg)](https://www.plumed-nest.org/browse.html?search=WRAPAROUND) | 

## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| AROUND | atoms | reference atoms |
| ATOMS | atoms | wrapped atoms |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| AROUND | input | none | reference atoms |
| ATOMS | input | none | wrapped atoms |
| STRIDE | compulsory | 1 |  the frequency with which molecules are reassembled |
| GROUPBY | compulsory | 1 |  group atoms so as not to break molecules |
| PAIR | optional | false |  Pair atoms in AROUND and ATOMS groups |

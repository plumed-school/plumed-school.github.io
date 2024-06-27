# Action: WRAPAROUND

| Description    | Usage |
|:--------:|:--------:|
| Rebuild periodic boundary conditions around chosen atoms. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 7 eggs](https://img.shields.io/badge/nest-7-green.svg)](https://www.plumed-nest.org/browse.html?search=WRAPAROUND) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 
| Keyword | Type | Default | Description |
|:-------:|:----:|:-------:|:-----------:|
| AROUND | input | none | reference atoms |
| ATOMS | input | none | wrapped atoms |
| STRIDE | compulsory | none |  the frequency with which molecules are reassembled |
| GROUPBY | compulsory | none |  group atoms so as not to break molecules |
| PAIR | optional | false |  Pair atoms in AROUND and ATOMS groups |

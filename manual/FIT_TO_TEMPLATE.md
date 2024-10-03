# [Action](actions.md): FIT_TO_TEMPLATE

| Description    | Usage |
|:--------|:--------:|
| This action is used to align a molecule to a template. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=FIT_TO_TEMPLATE)[![used in 17 eggs](https://img.shields.io/badge/nest-17-green.svg)](https://www.plumed-nest.org/browse.html?search=FIT_TO_TEMPLATE) | 

## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| STRIDE | compulsory | 1 |  the frequency with which molecules are reassembled |
| REFERENCE | compulsory | none | a file in pdb format containing the reference structure and the atoms involved in the CV |
| TYPE | compulsory | SIMPLE |  the manner in which RMSD alignment is performed |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |

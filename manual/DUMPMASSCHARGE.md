# Action: DUMPMASSCHARGE

| Description    | Usage |
|:--------|:--------:|
| Dump masses and charges on a selected file. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=DUMPMASSCHARGE) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the atom indices whose charges and masses you would like to print out |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the atom indices whose charges and masses you would like to print out |
| STRIDE | compulsory | none |  the frequency with which the atoms should be output |
| FILE | compulsory | none | file on which to output charges and masses |
| ONLY_MASSES | optional | false |  Only output masses to file |
| ONLY_CHARGES | optional | false |  Only output charges to file |

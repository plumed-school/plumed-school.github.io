# [Shortcut](shortcuts.md): READMASSCHARGE

| Description    | Usage |
|:--------|:--------:|
| Set the masses and charges from an input PDB file. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| mass | vector | the masses of the atoms in the system | 
| charges | vector | the masses of the atoms in the system | 


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| PDBFILE | compulsory | none | a pdb file that contains the masses and charges of the atoms in the beta and occupancy columns |
| FILE | optional | not used | input file that contains the masses and charges that should be used |

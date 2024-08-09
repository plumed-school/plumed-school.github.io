# Action: FUNNEL_PS

| Description    | Usage |
|:--------|:--------:|
| FUNNEL_PS implements the Funnel-Metadynamics (FM) technique in PLUMED 2. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 3 eggs](https://img.shields.io/badge/nest-3-green.svg)](https://www.plumed-nest.org/browse.html?search=FUNNEL_PS) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| lp | scalar | the position along the funnel line | 
| ld | scalar | the distance from the funnel line | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| LIGAND | atoms | This MUST be a single atom, normally the COM of the ligand |
| ANCHOR | atoms | Closest protein atom to the ligand, picked to avoid pbc problems during the simulation |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| LIGAND | input | none | This MUST be a single atom, normally the COM of the ligand |
| ANCHOR | input | none | Closest protein atom to the ligand, picked to avoid pbc problems during the simulation |
| REFERENCE | compulsory | none | a file in pdb format containing the structure you would like to align |
| POINTS | compulsory | none | 6 values defining x, y, and z of the 2 points used to construct the line |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| SQUARED-ROOT | optional | false |  Used to initialize the creation of the alignment variable |

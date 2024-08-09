# Action: UWALLS

| Description    | Usage |
|:--------|:--------:|
| Add lower walls to a vector of quantities | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=UWALLS) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| bias | scalar | the instantaneous value of the bias potential | 
| force2 | scalar | the instantaneous value of the squared force due to this bias potential | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| CATOMS | atoms | all the angles between the bonds that radiate out from these central atom are computed |
| GROUP | atoms | a list of angls between pairs of bonds connecting one of the atoms specified using the CATOM command and two of the atoms specified here are computed |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| CATOMS | input | none | all the angles between the bonds that radiate out from these central atom are computed |
| GROUP | input | none | a list of angls between pairs of bonds connecting one of the atoms specified using the CATOM command and two of the atoms specified here are computed |
| DATA | compulsory | none | the values you want to restrain |
| AT | compulsory | none | the radius of the sphere |
| KAPPA | compulsory | none | the force constant for the wall |
| OFFSET | compulsory | none |  the offset for the start of the wall |
| EXP | compulsory | none |  the powers for the walls |
| EPS | compulsory | none |  the values for s_i in the expression for a wall |
| SWITCH | compulsory | none | the switching function specifies that only those bonds that have a length that is less than a certain threshold are considered |

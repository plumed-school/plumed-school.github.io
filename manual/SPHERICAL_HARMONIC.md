# Action: SPHERICAL_HARMONIC

| Description    | Usage |
|:--------|:--------:|
| Calculate the values of all the spherical harmonic funtions for a particular value of l. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=SPHERICAL_HARMONIC)[![used in 9 eggs](https://img.shields.io/badge/nest-9-green.svg)](https://www.plumed-nest.org/browse.html?search=SPHERICAL_HARMONIC) | 

## Output components

This action calculates the quantities in the following table.  These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| rm | scalar | the real parts of the spherical harmonic values with the m value given | 
| im | scalar | the real parts of the spherical harmonic values with the m value given | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | scalar | the input to this function |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the input to this function |
| L | compulsory | none | the value of the angular momentum |

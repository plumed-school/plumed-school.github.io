# Action: CAVITY

| Description    | Usage |
|:--------|:--------:|
| This quantity can be used to calculate functions of the distribution of collective variables for the atoms that lie in a box defined by the positions of four atoms. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg)|
 | **output value** | **type** |
| vector of numbers between 0 and 1 that measure the degree to which each atom is within the volume of interest | scalar |

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| lessthan | scalar | LESS_THAN | the number of cvs in the region of interest that are less than a certain threshold | 
| morethan | scalar | MORE_THAN | the number of cvs in the region of interest that are more than a certain threshold | 
| between | scalar | BETWEEN | the number of cvs in the region of interest that are within a certain range | 
| sum | scalar | SUM | the sum of all the colvars weighted by the function that determines if we are in the region | 
| mean | scalar | MEAN | the average values of the colvar in the region of interest | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the group of atoms that you would like to investigate |
| BOX | atoms | the positions of four atoms that define spatial extent of the cavity |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the group of atoms that you would like to investigate |
| BOX | input | none | the positions of four atoms that define spatial extent of the cavity |
| SIGMA | compulsory | none | the width of the function to be used for kernel density estimation |
| KERNEL | compulsory | none |  the type of kernel function to be used |
| SERIAL | optional | false |  do the calculation in serial |
| OUTSIDE | optional | false |  calculate quantities for colvars that are on atoms outside the region of interest |
| PRINT_BOX | optional | false |  write out the positions of the corners of the box to an xyz file |
| FILE | optional | not used | the file on which to write out the box coordinates |
| UNITS | optional | not used |  the units in which to write out the corners of the box |
| DATA | optional | not used | the label of an action that calculates multicolvars |
| LESS_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are less than a certain threshold |
| MORE_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are greater that a certain threshold |
| BETWEEN | optional | not used | calculate the number of colvars that are inside the region of interest and that have a CV value that is between a particular set of bounds |
| SUM | optional | false |  calculate the sum of all the quantities |
| MEAN | optional | false |  calculate the average value of the colvar inside the region of interest |

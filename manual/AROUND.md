# [Shortcut](shortcuts.md): AROUND

| Description    | Usage |
|:--------|:--------:|
| This quantity can be used to calculate functions of the distribution of collective variables for the atoms that lie in a particular, user-specified part of of the cell. | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=AROUND)|
 | **output value** | **type** |
| sum of values of input CVs in regin of interest | scalar |

## Output components

This action can calculate the [values](pecifying_arguments.html) in the following table when the associated keyword is included in the input for the action. These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| lessthan | scalar | LESS_THAN | the number of cvs in the region of interest that are less than a certain threshold | 
| morethan | scalar | MORE_THAN | the number of cvs in the region of interest that are more than a certain threshold | 
| between | scalar | BETWEEN | the number of cvs in the region of interest that are within a certain range | 
| sum | scalar | SUM | the sum of all the colvars weighted by the function that determines if we are in the region | 
| mean | scalar | MEAN | the average values of the colvar in the region of interest | 


## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the group of atoms that you would like to investigate |
| ORIGIN | atoms | the atom whose vicinity we are interested in examining |
| ATOM | atoms | an alternative to ORIGIN |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the group of atoms that you would like to investigate |
| ORIGIN | input | none | the atom whose vicinity we are interested in examining |
| ATOM | input | none | an alternative to ORIGIN |
| SIGMA | compulsory | none | the width of the function to be used for kernel density estimation |
| KERNEL | compulsory | gaussian |  the type of kernel function to be used |
| XLOWER | compulsory | 0.0 |  the lower boundary in x relative to the x coordinate of the atom (0 indicates use full extent of box) |
| XUPPER | compulsory | 0.0 |  the upper boundary in x relative to the x coordinate of the atom (0 indicates use full extent of box) |
| YLOWER | compulsory | 0.0 |  the lower boundary in y relative to the y coordinate of the atom (0 indicates use full extent of box) |
| YUPPER | compulsory | 0.0 |  the upper boundary in y relative to the y coordinate of the atom (0 indicates use full extent of box) |
| ZLOWER | compulsory | 0.0 |  the lower boundary in z relative to the z coordinate of the atom (0 indicates use full extent of box) |
| ZUPPER | compulsory | 0.0 |  the upper boundary in z relative to the z coordinate of the atom (0 indicates use full extent of box) |
| SERIAL | optional | false |  do the calculation in serial |
| OUTSIDE | optional | false |  calculate quantities for colvars that are on atoms outside the region of interest |
| DATA | optional | not used | the label of an action that calculates multicolvars |
| LESS_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are less than a certain threshold |
| MORE_THAN | optional | not used | calcualte the number of colvars that are inside the region of interest and that are greater that a certain threshold |
| BETWEEN | optional | not used | calculate the number of colvars that are inside the region of interest and that have a CV value that is between a particular set of bounds |
| SUM | optional | false |  calculate the sum of all the quantities |
| MEAN | optional | false |  calculate the average value of the colvar inside the region of interest |

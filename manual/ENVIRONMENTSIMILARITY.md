# Action: ENVIRONMENTSIMILARITY

| Description    | Usage |
|:--------|:--------:|
| Measure how similar the environment around atoms is to that found in some reference crystal structure. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=ENVIRONMENTSIMILARITY)[![used in 9 eggs](https://img.shields.io/badge/nest-9-green.svg)](https://www.plumed-nest.org/browse.html?search=ENVIRONMENTSIMILARITY) | 

## Output components

This action can calculate the quantities in the following table when the associated keyword is included in the input for the action. These quantities can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the quantity required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| lessthan | scalar | LESS_THAN | the number of colvars that have a value less than a threshold | 
| morethan | scalar | MORE_THAN | the number of colvars that have a value more than a threshold | 
| altmin | scalar | ALT_MIN | the minimum value of the cv | 
| min | scalar | MIN | the minimum colvar | 
| max | scalar | MAX | the maximum colvar | 
| between | scalar | BETWEEN | the number of colvars that have a value that lies in a particular interval | 
| highest | scalar | HIGHEST | the largest of the colvars | 
| lowest | scalar | LOWEST | the smallest of the colvars | 
| sum | scalar | SUM | the sum of the colvars | 
| mean | scalar | MEAN | the mean of the colvars | 


## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| SPECIES | atoms | this keyword is used for colvars such as coordination number |
| SPECIESA | atoms | this keyword is used for colvars such as the coordination number |
| SPECIESB | atoms | this keyword is used for colvars such as the coordination number |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| SPECIES | input | none | this keyword is used for colvars such as coordination number |
| SPECIESA | input | none | this keyword is used for colvars such as the coordination number |
| SPECIESB | input | none | this keyword is used for colvars such as the coordination number |
| CRYSTAL_STRUCTURE | compulsory | none |  Targeted crystal structure |
| LATTICE_CONSTANTS | compulsory | none | Lattice constants |
| SIGMA | compulsory | none |  the width to use for the gaussian kernels |
| LCUTOFF | compulsory | none |  any atoms separated by less than this tolerance should be ignored |
| LAMBDA | compulsory | none |  Lambda parameter |
| CUTOFF | compulsory | none |  how many multiples of sigma would you like to consider beyond the maximum distance in the environment |
| REFERENCE | optional | not used | PDB files with relative distances from central atom |
| REFERENCE_ | optional | not used | PDB files with relative distances from central atom |
| ATOM_NAMES_FILE | optional | not used | PDB file with atom names for all atoms in SPECIES |
| LESS_THAN | optional | not used | calculate the number of variables that are less than a certain target value |
| MORE_THAN | optional | not used | calculate the number of variables that are more than a certain target value |
| ALT_MIN | optional | not used | calculate the minimum value |
| MIN | optional | not used | calculate the minimum value |
| MAX | optional | not used | calculate the maximum value |
| BETWEEN | optional | not used | calculate the number of values that are within a certain range |
| HIGHEST | optional | false |  this flag allows you to recover the highest of these variables |
| HISTOGRAM | optional | not used | calculate a discretized histogram of the distribution of values |
| LOWEST | optional | false |  this flag allows you to recover the lowest of these variables |
| SUM | optional | false |  calculate the sum of all the quantities |
| MEAN | optional | false |  calculate the mean of all the quantities |

# Action: FCCUBIC

| Description    | Usage |
|:--------|:--------:|
| Measure how similar the environment around atoms is to that found in a FCC structure. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=FCCUBIC)[![used in 3 eggs](https://img.shields.io/badge/nest-3-green.svg)](https://www.plumed-nest.org/browse.html?search=FCCUBIC) | 

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
| NN | compulsory | none |  The n parameter of the switching function  |
| MM | compulsory | none |  The m parameter of the switching function; 0 implies 2*NN |
| D_0 | compulsory | none |  The d_0 parameter of the switching function |
| R_0 | compulsory | none | The r_0 parameter of the switching function |
| FUNCTION | compulsory | none | the function of the bond vectors that you would like to evaluate |
| PHI | compulsory | none |  The Euler rotational angle phi |
| THETA | compulsory | none |  The Euler rotational angle theta |
| PSI | compulsory | none |  The Euler rotational angle psi |
| ALPHA | compulsory | none |  The alpha parameter of the angular function that is used for FCCUBIC |
| SWITCH | optional | not used | the switching function that it used in the construction of the contact matrix |
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
| LOWMEM | optional | false |  this flag does nothing and is present only to ensure back-compatibility |

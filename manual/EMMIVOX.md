# [Action](actions.md): EMMIVOX

| Description    | Usage |
|:--------|:--------:|
| Bayesian single-structure and ensemble refinement with cryo-EM maps. | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=EMMIVOX)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=EMMIVOX) | 

## Output components

This action can calculate the [values](pecifying_arguments.html) in the following table when the associated keyword is included in the input for the action. These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Keyword | Description |
|:-------|:-----|:----:|:-------|
| scoreb | scalar | default | Bayesian score | 
| scale | scalar | default | scale factor | 
| offset | scalar | default | offset | 
| accB | scalar | default | Bfactor MC acceptance | 
| kbt | scalar | default | temperature in energy unit | 
| corr | scalar | CORRELATION | correlation coefficient | 


## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | atoms used in the calculation of the density map, typically all heavy atoms |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | atoms used in the calculation of the density map, typically all heavy atoms |
| DATA_FILE | compulsory | none | file with cryo-EM map |
| RESOLUTION | compulsory | none | cryo-EM map resolution |
| NORM_DENSITY | compulsory | none | integral of experimental density |
| WRITE_STRIDE | compulsory | none | stride for writing status file |
| NUMERICAL_DERIVATIVES | optional | false |  calculate the derivatives for these quantities numerically |
| NOPBC | optional | false |  ignore the periodic boundary conditions when calculating distances |
| NL_DIST_CUTOFF | optional | not used | neighbor list distance cutoff |
| NL_GAUSS_CUTOFF | optional | not used | neighbor list Gaussian sigma cutoff |
| NL_STRIDE | optional | not used | neighbor list update frequency |
| SIGMA_MIN | optional | not used | minimum density error |
| DBFACT | optional | not used | Bfactor MC step |
| BFACT_MAX | optional | not used | Bfactor maximum value |
| MCBFACT_STRIDE | optional | not used | Bfactor MC stride |
| BFACT_SIGMA | optional | not used | Bfactor sigma prior |
| STATUS_FILE | optional | not used | write a file with all the data useful for restart |
| SCALE | optional | not used | scale factor |
| OFFSET | optional | not used | offset |
| TEMP | optional | not used | temperature |
| WRITE_MAP | optional | not used | file with model density |
| WRITE_MAP_STRIDE | optional | not used | stride for writing model density to file |
| NO_AVER | optional | false |  no ensemble averaging in multi-replica mode |
| CORRELATION | optional | false |  calculate correlation coefficient |
| GPU | optional | false |  calculate EMMIVOX on GPU with Libtorch |
| BFACT_NOCHAIN | optional | false |  Do not use chain ID for Bfactor MC |
| BFACT_READ | optional | false |  Read Bfactor on RESTART (automatic with DBFACT>0) |
| BFACT_MINIMIZE | optional | false |  Accept only moves that decrease energy |
| MARTINI | optional | false |  Use Martini scattering factors |

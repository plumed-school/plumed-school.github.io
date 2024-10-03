# [Action](actions.md): QUATERNION_PRODUCT_MATRIX

| Description    | Usage |
|:--------|:--------:|
| Calculate the outer product matrix from two vectors of quaternions | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)![used in 0 eggs](https://img.shields.io/badge/nest-0-red.svg) | 

## Output components

This action calculates the [values](pecifying_arguments.html) in the following table.  These [values](pecifying_arguments.html) can be referenced elsewhere in the input by using this Action's label followed by a dot and the name of the [value](pecifying_arguments.html) required from the list below.

| Name | Type | Description |
|:-------|:-----|:-------|
| w | matrix | the real component of quaternion | 
| i | matrix | the i component of the quaternion | 
| j | matrix | the j component of the quaternion | 
| k | matrix | the k component of the quaternion | 


## Input

The [arguments](specifying_arguments.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ARG | vector | the labels of the quaternion vectors that you are outer product of |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ARG | input | none | the labels of the quaternion vectors that you are outer product of |
| SERIAL | optional | false |  do the calculation in serial |

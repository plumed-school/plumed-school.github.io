# Action: BRIDGE

| Description    | Usage |
|:--------|:--------:|
| Calculate a matrix with elements equal to one if there is a bridging atom between the two atoms | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=BRIDGE)|
 | **output value** | **type** |
| the number of bridging atoms between the two groups | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| GROUP | atoms | the atoms for which you would like to calculate the adjacency matrix |
| GROUPA | atoms |  |
| GROUPB | atoms |  |
| BRIDGING_ATOMS | atoms | The list of atoms that can form the bridge between the two interesting parts of the structure |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| GROUP | input | none | the atoms for which you would like to calculate the adjacency matrix |
| GROUPA | input | none |  |
| GROUPB | input | none |  |
| BRIDGING_ATOMS | input | none | The list of atoms that can form the bridge between the two interesting parts of the structure |
| SWITCH | optional | not used | The parameters of the two switchingfunction in the above formula |
| SWITCHA | optional | not used | The switchingfunction on the distance between bridging atoms and the atoms in group A |
| SWITCHB | optional | not used | The switchingfunction on the distance between the bridging atoms and the atoms in group B |

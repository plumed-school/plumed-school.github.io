# Action: OUTPUT_CLUSTER

| Description    | Usage |
|:--------|:--------:|
| Output the indices of the atoms in one of the clusters identified by a clustering object | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 2 eggs](https://img.shields.io/badge/nest-2-green.svg)](https://www.plumed-nest.org/browse.html?search=OUTPUT_CLUSTER) | 

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | compulsory | none | the atoms for which clustering were performed |
| CLUSTERS | compulsory | none | the action that performed the clustering |
| CLUSTER | compulsory | none |  which cluster would you like to look at 1 is the largest cluster, 2 is the second largest, 3 is the the third largest and so on |
| STRIDE | compulsory | none |  the frequency with which you would like to output the atoms in the cluster |
| FILE | compulsory | none | the name of the file on which to output the details of the cluster |

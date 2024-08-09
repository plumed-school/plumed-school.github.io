# Action: PAIRENTROPY

| Description    | Usage |
|:--------|:--------:|
| Calculate the KL Entropy from the radial distribution function | [![used in 1 tutorials](https://img.shields.io/badge/tutorials-1-green.svg)](https://www.plumed-tutorials.org/browse.html?search=PAIRENTROPY)[![used in 4 eggs](https://img.shields.io/badge/nest-4-green.svg)](https://www.plumed-nest.org/browse.html?search=PAIRENTROPY)|
 | **output value** | **type** |
| the KL-entropy that is computed from the radial distribution function | scalar |

## Input

The input for this action is specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| GROUP | atoms |  |
| GROUPA | atoms |  |
| GROUPB | atoms |  |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the keywords and options that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| GROUP | input | none |  |
| GROUPA | input | none |  |
| GROUPB | input | none |  |
| GRID_BIN | compulsory | none | the number of bins to use when computing the RDF |
| KERNEL | compulsory | none |  the type of kernel to use for computing the histograms for the RDF |
| CUTOFF | compulsory | none |  the cutoff at which to stop evaluating the kernel functions is set equal to sqrt(2*x)*bandwidth in each direction where x is this number |
| MAXR | compulsory | none | the maximum distance to use for the rdf |
| BANDWIDTH | compulsory | none | the bandwidths for kernel density esimtation |
| CLEAR | compulsory | none |  the frequency with which to clear the estimate of the rdf |
| STRIDE | compulsory | none |  the frequency with which to compute the rdf and accumulate averages |
| DENSITY | optional | not used | the reference density to use when normalizing the RDF |

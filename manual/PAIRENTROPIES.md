# [Shortcut](shortcuts.md): PAIRENTROPIES

| Description    | Usage |
|:--------|:--------:|
| Calculate the KL entropy from the RDF around each of the atoms | ![used in 0 tutorials](https://img.shields.io/badge/tutorials-0-red.svg)[![used in 1 eggs](https://img.shields.io/badge/nest-1-green.svg)](https://www.plumed-nest.org/browse.html?search=PAIRENTROPIES)|
 | **output value** | **type** |
| the a vector containing the KL-entropy that is computed from the radial distribution function around each of the atoms in the input | vector |

## Input

The [atoms](specifying_atoms.html) that serve as the input for this action are specified using one or more of the keywords in the following table.

| Keyword |  Type | Description |
|:--------|:------:|:-----------|
| ATOMS | atoms | the atoms that you would like to compute the entropies for |


## Further details and examples 
Information for the manual from the code would go in here 
## Syntax 
The following table describes the [keywords and options](parsing.md) that can be used with this action 

| Keyword | Type | Default | Description |
|:-------|:----:|:-------:|:-----------|
| ATOMS | input | none | the atoms that you would like to compute the entropies for |
| GRID_BIN | compulsory | none | the number of bins to use when computing the RDF |
| KERNEL | compulsory | GAUSSIAN |  the type of kernel to use for computing the histograms for the RDF |
| CUTOFF | compulsory | 6.25 |  the cutoff at which to stop evaluating the kernel functions is set equal to sqrt(2*x)*bandwidth in each direction where x is this number |
| MAXR | compulsory | none | the maximum distance to use for the rdf |
| BANDWIDTH | compulsory | none | the bandwidths for kernel density esimtation |
| CLEAR | compulsory | 1 |  the frequency with which to clear the estimate of the rdf |
| STRIDE | compulsory | 1 |  the frequency with which to compute the rdf and accumulate averages |
| DENSITY | optional | not used | the reference density to use when normalizing the RDF |

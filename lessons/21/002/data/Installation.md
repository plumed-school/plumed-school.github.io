# Installation advice

Everything in this tutorial can be performed using PLUMED only. In other words, none of the exercises in this tutorial require 
you to run an molecular dynamics code and call PLUMED from it. All the molecular dynamics in this tutorial is performed using PLUMED's
internal MD code - `simplemd`. You thus only need to install PLUMED using the instructions you can find 
[here](https://www.plumed-tutorials.org/lessons/20/001/data/NAVIGATION.html).  

I think the quickest way to get PLUMED running on your computer so you can do the tutorial is to install it with [conda](https://anaconda.org).  
You can create and activate a conda environment to run the tutorial exercises by issuing the following commands:

```bash
conda create --name masterclass212-env python=3.13
conda activate masterclass212-env
```   

You can then install PLUMED into this environment with the following command:

```bash
conda install -c conda-forge plumed
```

You should then be able to run all the commands that use PLUMED in the tutorial.

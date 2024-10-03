# PLUMED Masterclass 22.3: OPES method

## Origin

This masterclass was authored by Michele Invernizzi on February 28, 2022

## Aims

This Masterclass is an introduction to the [OPES](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s.html) method and its PLUMED implementation.

## Objectives

Once this Masterclass is completed, you will be able to:

- Perform OPES simulations and analyse the results.
- Use [OPES_EXPANDED](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html) to sample different generalized ensembles
- Test the effect of various [OPES_METAD](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html) input options
- Understand the typical use-case for [OPES_METAD_EXPLORE](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d__e_x_p_l_o_r_e.html)

## Prerequisites

We assume that you are familiar with PLUMED, metadynamics, umbrella sampling, and replica exchange.
If you are not, the 2021 PLUMED Masterclass from the graph is a good place to start.  We would also recommend reading
the papers that are linked in the graph.

## Overview of the theory

The OPES method is an evolution of Metadynamics that also incorporates some of the ideas of the [VES](https://www.plumed.org/doc-master/user-doc/html/_v_e_s.html) method.
OPES is designed to be simple to use and robust with respect to suboptimal collective variables.
Compared to metadynamics, it is faster in converging to a quasi-static bias and it handles multi-dimensional collective variables more efficiently.

The theory for the OPES method is presented in the papers that we give in the graph for this tutorial.
A short overview can also be found in the PLUMED documentation at [OPES](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s.html), [OPES_EXPANDED](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html), [OPES_METAD](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html), and [OPES_METAD_EXPLORE](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d__e_x_p_l_o_r_e.html).

## Setting up the software

For this Masterclass we will use GROMACS 2020.6 patched with PLUMED 2.8, with the OPES module and MPI enabled.
The easiest way to install all the software needed is to use the `plumed-masterclass-2022` conda environment, as described [here](https://github.com/plumed/masterclass-2022).

## Resources

The data needed to complete the exercises of this Masterclass can be found on [GitHub](https://github.com/invemichele/masterclass-22-03).
You can clone this repository locally on your machine with the usual command:

````
git clone https://github.com/invemichele/masterclass-22-03.git
````

The repository contains all the data to run the simulations, together with the scripts to analyse them.
It also contains some annotated [Jupyter notebooks](https://github.com/invemichele/masterclass-22-03/tree/master/notebooks), that will guide us through this tutorial.
Most of the information can be found there, and this page is mainly meant as an overview of the content of the notebooks.

As done in some previous masterclass, we will play with a toy system, the small alanine dipeptide molecule in vacuum (ala2).
It has the advantage of being a well-known system, cheap to simulate and with a higher level of complexity compared to a 2D model potential as the one used in this other [OPES_METAD](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html).
Ala2 has two main metastable basins which can be identified by a very efficient collective variable (CV), the $\phi$ torsional angle.
Here is its free energy surface (FES) as a function of the $\phi$ and $\psi$ angles:

![Alanine dipeptide free energy surface along the Ramachandran angles](figures/masterclass-22-03-ala2_FES.png)

_All the exercises have been tested with PLUMED version 2.8.0 and GROMACS 2020.6_

## Exercise 1: Sampling expanded ensembles with OPES

We start by using OPES to sample expanded ensembles.
This probably is not a familiar application of adaptive-bias enhanced sampling for most of PLUMED users, so we will first introduce some theory background.

### 1.1 Multithermal simulations

The first example we consider is a multithermal simulation of alanine dipeptide.
One can use replica exchange to perform a parallel tempering simulation and sample the two metastable states of alanine dipeptide.
Here instead, we want to sample the same multithermal distribution not by combining simulations at different temperatures, but by adding a bias potential to a single simulation.
You can find details on the relevant theory by searching through the graph for this tutorial.

<details>
    <summary><u>Click to expand</u></summary>

We choose 3 temperatures $T_0, T_1, T_2$, ranging from 300 K to 1000 K, and setup our GROMACS simulation to run at $T_0=300$ K.
Our target distribution is then:

$$p^{\text{tg}}(\mathbf{x})=\frac{1}{3}\left[\frac{e^{-\frac{1}{k_BT_0}U(\mathbf{x})}}{Z_0}+ \frac{e^{-\frac{1}{k_BT_1}U(\mathbf{x})}}{Z_1}+\frac{e^{-\frac{1}{k_BT_2}U(\mathbf{x})}}{Z_2}\right] .$$

This can be rewritten highlighting $P(\mathbf{x})$

$$p^{\text{tg}}(\mathbf{x})=P(\mathbf{x})\frac{1}{3}\left[1+ e^{-\left(\frac{1}{k_BT_1}-\frac{1}{k_BT_0}\right)U(\mathbf{x})}\frac{Z_0}{Z_1}+e^{-\left(\frac{1}{k_BT_2}-\frac{1}{k_BT_0}\right)U(\mathbf{x})}\frac{Z_0}{Z_2}\right] ,$$

and then using $\Delta F_i = -k_B T_0 \log \frac{Z_i}{Z_0}$:

$$p^{\text{tg}}(\mathbf{x})=P(\mathbf{x})\frac{1}{3}\left[1+ e^{-\frac{1-T_0/T_1}{k_BT_0}U(\mathbf{x})+\frac{1}{k_BT_0}\Delta F_1}+e^{-\frac{1-T_0/T_2}{k_BT_0}U(\mathbf{x})+\frac{1}{k_BT_0}\Delta F_2}\right] .$$

So we just need to know $\Delta F_1$ and $\Delta F_2$, and we can sample the target multithermal distribution by using the following bias:

$$V(U) = - k_B T_0 \log \frac{1}{3}\left[1+ e^{-\frac{1-T_0/T_1}{k_BT_0}U(\mathbf{x})+\frac{1}{k_BT_0}\Delta F_1}+e^{-\frac{1-T_0/T_2}{k_BT_0}U(\mathbf{x})+\frac{1}{k_BT_0}\Delta F_2}\right] ,$$

that is a function only of the potential energy $U=U(\mathbf{x})$.
In the OPES spirit, we estimate on-the-fly these free energy differences using a simple reweighting, and iteratively reach the target distribution.

The final bias expression is determined by these quantities $\frac{1-T_0/T_i}{k_BT_0}U(\mathbf{x})$, that we call [expansion_cv](https://www.plumed.org/doc-master/user-doc/html/expansion__c_v.html) (ECVs).
There are several types of expanded ensembles that might be of interest, and in order to sample them with OPES one simply needs to find the explicit form of the corresponding ECVs.
To sample the same expanded ensemble with replica exchange, one has to run a different replica of the system for each of the ECVs.
</details>

Enough equations, here is the plumed input file we need to run this multithermal simulation:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_INSTRUCTIONS.md_working_1.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="INSTRUCTIONS.md_working_1.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="INSTRUCTIONS.md_working_1.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="INSTRUCTIONS.md_working_1.datene" onclick='showPath("INSTRUCTIONS.md_working_1.dat","INSTRUCTIONS.md_working_1.datene","INSTRUCTIONS.md_working_1.datene","black")'>ene</b><span style="display:none;" id="INSTRUCTIONS.md_working_1.datene">The ENERGY action with label <b>ene</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ene</td><td width="5%"><font color="black">scalar</font></td><td>the internal energy</td></tr></table></span>: <div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div>
<span id="INSTRUCTIONS.md_working_1.datdefecv_short"><b name="INSTRUCTIONS.md_working_1.datecv" onclick='showPath("INSTRUCTIONS.md_working_1.dat","INSTRUCTIONS.md_working_1.datecv","INSTRUCTIONS.md_working_1.datecv","black")'>ecv</b><span style="display:none;" id="INSTRUCTIONS.md_working_1.datecv">The ECV_MULTITHERMAL action with label <b>ecv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ecv.ene</td><td width="5%"><font color="black">scalar</font></td><td>the value of the argument named ene</td></tr></table></span>: <div class="tooltip" style="color:green">ECV_MULTITHERMAL<div class="right">Expand a simulation to sample multiple temperatures simultaneously. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_1.datdefecv");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__m_u_l_t_i_t_h_e_r_m_a_l.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the internal energy of the system<i></i></div></div>=<b name="INSTRUCTIONS.md_working_1.datene">ene</b> <div class="tooltip">TEMP_MIN<div class="right">the minimum of the temperature range<i></i></div></div>=300 <div class="tooltip">TEMP_MAX<div class="right">the maximum of the temperature range<i></i></div></div>=1000 <div class="tooltip">TEMP_STEPS<div class="right">the number of steps in temperature<i></i></div></div>=3
</span><span id="INSTRUCTIONS.md_working_1.datdefecv_long" style="display:none;"><b name="INSTRUCTIONS.md_working_1.datecv" onclick='showPath("INSTRUCTIONS.md_working_1.dat","INSTRUCTIONS.md_working_1.datecv","INSTRUCTIONS.md_working_1.datecv","black")'>ecv</b>: <div class="tooltip" style="color:green">ECV_MULTITHERMAL<div class="right">Expand a simulation to sample multiple temperatures simultaneously. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_1.datdefecv");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__m_u_l_t_i_t_h_e_r_m_a_l.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the internal energy of the system<i></i></div></div>=<b name="INSTRUCTIONS.md_working_1.datene">ene</b> <div class="tooltip">TEMP_MIN<div class="right">the minimum of the temperature range<i></i></div></div>=300 <div class="tooltip">TEMP_MAX<div class="right">the maximum of the temperature range<i></i></div></div>=1000 <div class="tooltip">TEMP_STEPS<div class="right">the number of steps in temperature<i></i></div></div>=3  <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=-1
</span><span id="INSTRUCTIONS.md_working_1.datdefopes_short"><b name="INSTRUCTIONS.md_working_1.datopes" onclick='showPath("INSTRUCTIONS.md_working_1.dat","INSTRUCTIONS.md_working_1.datopes","INSTRUCTIONS.md_working_1.datopes","black")'>opes</b><span style="display:none;" id="INSTRUCTIONS.md_working_1.datopes">The OPES_EXPANDED action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">OPES_EXPANDED<div class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_1.datdefopes");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the ECVs that define the expansion<i></i></div></div>=<b name="INSTRUCTIONS.md_working_1.datecv">ecv.ene</b> <div class="tooltip">PACE<div class="right">how often the bias is updated<i></i></div></div>=500
</span><span id="INSTRUCTIONS.md_working_1.datdefopes_long" style="display:none;"><b name="INSTRUCTIONS.md_working_1.datopes" onclick='showPath("INSTRUCTIONS.md_working_1.dat","INSTRUCTIONS.md_working_1.datopes","INSTRUCTIONS.md_working_1.datopes","black")'>opes</b>: <div class="tooltip" style="color:green">OPES_EXPANDED<div class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_1.datdefopes");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the ECVs that define the expansion<i></i></div></div>=<b name="INSTRUCTIONS.md_working_1.datecv">ecv.ene</b> <div class="tooltip">PACE<div class="right">how often the bias is updated<i></i></div></div>=500  <div class="tooltip">OBSERVATION_STEPS<div class="right"> number of unbiased initial PACE steps to collect statistics for initialization<i></i></div></div>=100 <div class="tooltip">FILE<div class="right"> a file with the estimate of the relative Delta F for each component of the target and of the global c(t)<i></i></div></div>=DELTAFS <div class="tooltip">PRINT_STRIDE<div class="right"> stride for printing to DELTAFS file, in units of PACE<i></i></div></div>=100
</span></pre>
 {% endraw %} 

We use the [OPES_EXPANDED](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html) bias action, with a multithermal expansion defined by the [ECV_MULTITHERMAL](https://www.plumed.org/doc-master/user-doc/html/_e_c_v__m_u_l_t_i_t_h_e_r_m_a_l.html) action.
The resulting bias is a function of the potential energy, and is updated every 500 MD steps.

In the notebook we show the shape of the resulting bias, how to check for convergence and how to reweight for estimating the free energy at different temperatures.
We also explain a simple procedure that is used to automatically set a reasonable number of temperature steps, if TEMP_STEPS is not provided.

### Multiumbrella simulations

Next, we present another expanded ensemble that can also be sampled by replica exchange.
We call it multiumbrella and it is composed by all the distributions sampled by a typical multiple windows umbrella sampling simulation.
In this kind of umbrella sampling, one chooses a CV and runs several simulations each one with a parabolic bias potential at a different CV location.
We can use OPES to sample an expanded target distribution that is composed of all of these combined.

In multiple windows umbrella sampling, the free energy difference between the windows is estimated during postprocessing (e.g. with WHAM), in OPES this is done on-the-fly at simulation time.
The main advantages are that choosing the number and location of the umbrellas becomes easier, and having a single longer simulation can also help with sampling orthogonal slow degrees of freedom.

We choose as CV the $\phi$ angle.
The ECVs we need for this type of expansion are the following:

$$\Delta u_i = \frac{(\phi-\phi_i)^2}{2\sigma^2} ,$$

where $\phi_i$ are the fixed centers of the umbrellas and $\sigma$ determines their width.
Usually in umbrella sampling another parameter is used, $k=1/\sqrt{\sigma}$, but we will see in the notebook why we made a different choice.

The plumed input we need might look like this:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_INSTRUCTIONS.md_working_2.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="INSTRUCTIONS.md_working_2.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="INSTRUCTIONS.md_working_2.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="INSTRUCTIONS.md_working_2.datphi" onclick='showPath("INSTRUCTIONS.md_working_2.dat","INSTRUCTIONS.md_working_2.datphi","INSTRUCTIONS.md_working_2.datphi","black")'>phi</b><span style="display:none;" id="INSTRUCTIONS.md_working_2.datphi">The TORSION action with label <b>phi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">phi</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=5,7,9,15
<span id="INSTRUCTIONS.md_working_2.datdefecv_short"><b name="INSTRUCTIONS.md_working_2.datecv" onclick='showPath("INSTRUCTIONS.md_working_2.dat","INSTRUCTIONS.md_working_2.datecv","INSTRUCTIONS.md_working_2.datecv","black")'>ecv</b><span style="display:none;" id="INSTRUCTIONS.md_working_2.datecv">The ECV_UMBRELLAS_LINE action with label <b>ecv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ecv.phi</td><td width="5%"><font color="black">scalar</font></td><td>the value of the argument named phi</td></tr></table></span>: <div class="tooltip" style="color:green">ECV_UMBRELLAS_LINE<div class="right">Target a multiumbrella ensemble, by combining systems each with a parabolic bias potential at a different location. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_2.datdefecv");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__u_m_b_r_e_l_l_a_s__l_i_n_e.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalar values that are input to this action<i></i></div></div>=<b name="INSTRUCTIONS.md_working_2.datphi">phi</b> <div class="tooltip">CV_MIN<div class="right">the minimum of the CV range to be explored<i></i></div></div>=-pi <div class="tooltip">CV_MAX<div class="right">the maximum of the CV range to be explored<i></i></div></div>=pi <div class="tooltip">SIGMA<div class="right">sigma of the umbrella Gaussians<i></i></div></div>=0.2
</span><span id="INSTRUCTIONS.md_working_2.datdefecv_long" style="display:none;"><b name="INSTRUCTIONS.md_working_2.datecv" onclick='showPath("INSTRUCTIONS.md_working_2.dat","INSTRUCTIONS.md_working_2.datecv","INSTRUCTIONS.md_working_2.datecv","black")'>ecv</b>: <div class="tooltip" style="color:green">ECV_UMBRELLAS_LINE<div class="right">Target a multiumbrella ensemble, by combining systems each with a parabolic bias potential at a different location. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_2.datdefecv");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__u_m_b_r_e_l_l_a_s__l_i_n_e.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalar values that are input to this action<i></i></div></div>=<b name="INSTRUCTIONS.md_working_2.datphi">phi</b> <div class="tooltip">CV_MIN<div class="right">the minimum of the CV range to be explored<i></i></div></div>=-pi <div class="tooltip">CV_MAX<div class="right">the maximum of the CV range to be explored<i></i></div></div>=pi <div class="tooltip">SIGMA<div class="right">sigma of the umbrella Gaussians<i></i></div></div>=0.2  <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=-1 <div class="tooltip">SPACING<div class="right"> the distance between umbrellas, in units of SIGMA<i></i></div></div>=1
</span><span id="INSTRUCTIONS.md_working_2.datdefopes_short"><b name="INSTRUCTIONS.md_working_2.datopes" onclick='showPath("INSTRUCTIONS.md_working_2.dat","INSTRUCTIONS.md_working_2.datopes","INSTRUCTIONS.md_working_2.datopes","black")'>opes</b><span style="display:none;" id="INSTRUCTIONS.md_working_2.datopes">The OPES_EXPANDED action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">OPES_EXPANDED<div class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_2.datdefopes");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the ECVs that define the expansion<i></i></div></div>=<b name="INSTRUCTIONS.md_working_2.datecv">ecv.phi</b> <div class="tooltip">PACE<div class="right">how often the bias is updated<i></i></div></div>=500
</span><span id="INSTRUCTIONS.md_working_2.datdefopes_long" style="display:none;"><b name="INSTRUCTIONS.md_working_2.datopes" onclick='showPath("INSTRUCTIONS.md_working_2.dat","INSTRUCTIONS.md_working_2.datopes","INSTRUCTIONS.md_working_2.datopes","black")'>opes</b>: <div class="tooltip" style="color:green">OPES_EXPANDED<div class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_2.datdefopes");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the ECVs that define the expansion<i></i></div></div>=<b name="INSTRUCTIONS.md_working_2.datecv">ecv.phi</b> <div class="tooltip">PACE<div class="right">how often the bias is updated<i></i></div></div>=500  <div class="tooltip">OBSERVATION_STEPS<div class="right"> number of unbiased initial PACE steps to collect statistics for initialization<i></i></div></div>=100 <div class="tooltip">FILE<div class="right"> a file with the estimate of the relative Delta F for each component of the target and of the global c(t)<i></i></div></div>=DELTAFS <div class="tooltip">PRINT_STRIDE<div class="right"> stride for printing to DELTAFS file, in units of PACE<i></i></div></div>=100
</span></pre>
 {% endraw %} 

This places umbrellas uniformly along $\phi$, each one separated by a distance of one $\sigma$.
We can make them less close to each with the keyword SPACING.
We can also provide a guess of the maximum free energy BARRIER we need to overcome, it can help speed up convergence.

In the notebook we show what kind of sampling this input provides, and invite you to play around with the parameters, to get a sense of what each option does.
We also perform reweighting to obtain a FES estimate.
This reweighting is done with kernel density estimation (similarly to plumed [HISTOGRAM](https://www.plumed.org/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html) function), and is interesting to see the effect of changing the bandwidth parameter.


### 1.3 Combined multithermal and multiumbrella simulations

Another advantage of using OPES to sample expanded ensembles is that it makes it very easy to combine them.
We show this by running a combined multithermal and multiumbrella simulation of alanine dipeptide.

Using the multithermal expansion, we were able to sample both metastable states, but not very efficiently.
With the multiumbrella target distribution we have many transitions, but we sample only at 300 K.
By combining these two expansions we obtain the best of both, with frequent transitions and an efficient reweighting over a whole range of temperatures.

The drawback? We might have to deal with a lot of ECVs!
However, while in a replica exchange scheme each ECV requires its own replica, with OPES we are free to use just one, or choose any number of parallel replica, in a multiple walkers scheme.

The way we combine expansions is to create a grid with all possible combinations of temperature ECVs and umbrella ECVs.
So, if we have 10 ECVs for the temperature expansion and 20 for the multiumbrella one, we end up with 200 combined ECVs.
This will become clearer once we look at the notebook and the simulation output.

From the point of view of the plumed input things are quite straightforward.
For a combined multithermal-multiumbrella simulation it should look similar to this one:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_INSTRUCTIONS.md_working_3.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="INSTRUCTIONS.md_working_3.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="INSTRUCTIONS.md_working_3.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># temperature expansion, based on energy</span>
<b name="INSTRUCTIONS.md_working_3.datene" onclick='showPath("INSTRUCTIONS.md_working_3.dat","INSTRUCTIONS.md_working_3.datene","INSTRUCTIONS.md_working_3.datene","black")'>ene</b><span style="display:none;" id="INSTRUCTIONS.md_working_3.datene">The ENERGY action with label <b>ene</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ene</td><td width="5%"><font color="black">scalar</font></td><td>the internal energy</td></tr></table></span>: <div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div>
<span id="INSTRUCTIONS.md_working_3.datdefecv_mt_short"><b name="INSTRUCTIONS.md_working_3.datecv_mt" onclick='showPath("INSTRUCTIONS.md_working_3.dat","INSTRUCTIONS.md_working_3.datecv_mt","INSTRUCTIONS.md_working_3.datecv_mt","black")'>ecv_mt</b><span style="display:none;" id="INSTRUCTIONS.md_working_3.datecv_mt">The ECV_MULTITHERMAL action with label <b>ecv_mt</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ecv_mt.ene</td><td width="5%"><font color="black">scalar</font></td><td>the value of the argument named ene</td></tr></table></span>: <div class="tooltip" style="color:green">ECV_MULTITHERMAL<div class="right">Expand a simulation to sample multiple temperatures simultaneously. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_3.datdefecv_mt");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__m_u_l_t_i_t_h_e_r_m_a_l.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the internal energy of the system<i></i></div></div>=<b name="INSTRUCTIONS.md_working_3.datene">ene</b> <div class="tooltip">TEMP_MIN<div class="right">the minimum of the temperature range<i></i></div></div>=300 <div class="tooltip">TEMP_MAX<div class="right">the maximum of the temperature range<i></i></div></div>=1000
</span><span id="INSTRUCTIONS.md_working_3.datdefecv_mt_long" style="display:none;"><b name="INSTRUCTIONS.md_working_3.datecv_mt" onclick='showPath("INSTRUCTIONS.md_working_3.dat","INSTRUCTIONS.md_working_3.datecv_mt","INSTRUCTIONS.md_working_3.datecv_mt","black")'>ecv_mt</b>: <div class="tooltip" style="color:green">ECV_MULTITHERMAL<div class="right">Expand a simulation to sample multiple temperatures simultaneously. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_3.datdefecv_mt");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__m_u_l_t_i_t_h_e_r_m_a_l.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the internal energy of the system<i></i></div></div>=<b name="INSTRUCTIONS.md_working_3.datene">ene</b> <div class="tooltip">TEMP_MIN<div class="right">the minimum of the temperature range<i></i></div></div>=300 <div class="tooltip">TEMP_MAX<div class="right">the maximum of the temperature range<i></i></div></div>=1000  <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=-1
</span><span style="color:blue" class="comment"># multiumbrella expansion, based on phi</span>
<b name="INSTRUCTIONS.md_working_3.datphi" onclick='showPath("INSTRUCTIONS.md_working_3.dat","INSTRUCTIONS.md_working_3.datphi","INSTRUCTIONS.md_working_3.datphi","black")'>phi</b><span style="display:none;" id="INSTRUCTIONS.md_working_3.datphi">The TORSION action with label <b>phi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">phi</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=5,7,9,15
<span id="INSTRUCTIONS.md_working_3.datdefecv_mu_short"><b name="INSTRUCTIONS.md_working_3.datecv_mu" onclick='showPath("INSTRUCTIONS.md_working_3.dat","INSTRUCTIONS.md_working_3.datecv_mu","INSTRUCTIONS.md_working_3.datecv_mu","black")'>ecv_mu</b><span style="display:none;" id="INSTRUCTIONS.md_working_3.datecv_mu">The ECV_UMBRELLAS_LINE action with label <b>ecv_mu</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ecv_mu.phi</td><td width="5%"><font color="black">scalar</font></td><td>the value of the argument named phi</td></tr></table></span>: <div class="tooltip" style="color:green">ECV_UMBRELLAS_LINE<div class="right">Target a multiumbrella ensemble, by combining systems each with a parabolic bias potential at a different location. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_3.datdefecv_mu");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__u_m_b_r_e_l_l_a_s__l_i_n_e.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalar values that are input to this action<i></i></div></div>=<b name="INSTRUCTIONS.md_working_3.datphi">phi</b> <div class="tooltip">CV_MIN<div class="right">the minimum of the CV range to be explored<i></i></div></div>=-pi <div class="tooltip">CV_MAX<div class="right">the maximum of the CV range to be explored<i></i></div></div>=pi <div class="tooltip">SIGMA<div class="right">sigma of the umbrella Gaussians<i></i></div></div>=0.2
</span><span id="INSTRUCTIONS.md_working_3.datdefecv_mu_long" style="display:none;"><b name="INSTRUCTIONS.md_working_3.datecv_mu" onclick='showPath("INSTRUCTIONS.md_working_3.dat","INSTRUCTIONS.md_working_3.datecv_mu","INSTRUCTIONS.md_working_3.datecv_mu","black")'>ecv_mu</b>: <div class="tooltip" style="color:green">ECV_UMBRELLAS_LINE<div class="right">Target a multiumbrella ensemble, by combining systems each with a parabolic bias potential at a different location. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_3.datdefecv_mu");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__u_m_b_r_e_l_l_a_s__l_i_n_e.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalar values that are input to this action<i></i></div></div>=<b name="INSTRUCTIONS.md_working_3.datphi">phi</b> <div class="tooltip">CV_MIN<div class="right">the minimum of the CV range to be explored<i></i></div></div>=-pi <div class="tooltip">CV_MAX<div class="right">the maximum of the CV range to be explored<i></i></div></div>=pi <div class="tooltip">SIGMA<div class="right">sigma of the umbrella Gaussians<i></i></div></div>=0.2  <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=-1 <div class="tooltip">SPACING<div class="right"> the distance between umbrellas, in units of SIGMA<i></i></div></div>=1
</span><span style="color:blue" class="comment"># the OPES bias combines them</span>
<span id="INSTRUCTIONS.md_working_3.datdefopes_short"><b name="INSTRUCTIONS.md_working_3.datopes" onclick='showPath("INSTRUCTIONS.md_working_3.dat","INSTRUCTIONS.md_working_3.datopes","INSTRUCTIONS.md_working_3.datopes","black")'>opes</b><span style="display:none;" id="INSTRUCTIONS.md_working_3.datopes">The OPES_EXPANDED action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">OPES_EXPANDED<div class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_3.datdefopes");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the ECVs that define the expansion<i></i></div></div>=<b name="INSTRUCTIONS.md_working_3.datecv_mt">ecv_mt.ene</b>,<b name="INSTRUCTIONS.md_working_3.datecv_mu">ecv_mu.phi</b> <div class="tooltip">PACE<div class="right">how often the bias is updated<i></i></div></div>=500
</span><span id="INSTRUCTIONS.md_working_3.datdefopes_long" style="display:none;"><b name="INSTRUCTIONS.md_working_3.datopes" onclick='showPath("INSTRUCTIONS.md_working_3.dat","INSTRUCTIONS.md_working_3.datopes","INSTRUCTIONS.md_working_3.datopes","black")'>opes</b>: <div class="tooltip" style="color:green">OPES_EXPANDED<div class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_3.datdefopes");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the ECVs that define the expansion<i></i></div></div>=<b name="INSTRUCTIONS.md_working_3.datecv_mt">ecv_mt.ene</b>,<b name="INSTRUCTIONS.md_working_3.datecv_mu">ecv_mu.phi</b> <div class="tooltip">PACE<div class="right">how often the bias is updated<i></i></div></div>=500  <div class="tooltip">OBSERVATION_STEPS<div class="right"> number of unbiased initial PACE steps to collect statistics for initialization<i></i></div></div>=100 <div class="tooltip">FILE<div class="right"> a file with the estimate of the relative Delta F for each component of the target and of the global c(t)<i></i></div></div>=DELTAFS <div class="tooltip">PRINT_STRIDE<div class="right"> stride for printing to DELTAFS file, in units of PACE<i></i></div></div>=100
</span></pre>
 {% endraw %} 

To fully appreciate the strength of combining these two different expansions, one can run the same simulations but using the $\psi$ angle instead of $\phi$, and see what happens.

## Exercise 2: OPES for metadynamics-like simulations

We now use OPES to perform biased simulations very similar to those of metadynamics.
We will sample a well-tempered distribution along a chosen set of collective variables.

### 2.1 Biasing a good CV

We start by biasing the $\phi$ angle, which is known to be a good CV for alanine dipeptide.
Here is how the FES along this CV looks like:

![Alanine dipeptide free energy surface along one of its torsional angles](figures/masterclass-22-03-ala2_FESphi.png)

We use this simple example to get familiar with [OPES_METAD](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html), its input parameter and output quantities.
We also compare it with well-tempered metadynamics, and we start to see how this two methods differ.

This also gives us the opportunity of using some of the postprocessing scripts for OPES.
For OPES, there is not yet a tool similar to the [sum_hills](https://www.plumed.org/doc-master/user-doc/html/sum_hills.html), but we can obtain the same result with simple python scripts and by dumping the state of the simulation through the STATE_WFILE keyword.
This STATE file contains the compressed kernels used by OPES at a given time to represent the probability distribution, and thus the bias.

### Biasing two good CVs

Next, we move to biasing both the Ramachandran angles of ala2.
A minimal plumed input to do this is the following:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_INSTRUCTIONS.md_working_4.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="INSTRUCTIONS.md_working_4.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="INSTRUCTIONS.md_working_4.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="INSTRUCTIONS.md_working_4.datphi" onclick='showPath("INSTRUCTIONS.md_working_4.dat","INSTRUCTIONS.md_working_4.datphi","INSTRUCTIONS.md_working_4.datphi","black")'>phi</b><span style="display:none;" id="INSTRUCTIONS.md_working_4.datphi">The TORSION action with label <b>phi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">phi</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=5,7,9,15
<b name="INSTRUCTIONS.md_working_4.datpsi" onclick='showPath("INSTRUCTIONS.md_working_4.dat","INSTRUCTIONS.md_working_4.datpsi","INSTRUCTIONS.md_working_4.datpsi","black")'>psi</b><span style="display:none;" id="INSTRUCTIONS.md_working_4.datpsi">The TORSION action with label <b>psi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">psi</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=7,9,15,17
<span id="INSTRUCTIONS.md_working_4.datdefopes_short"><b name="INSTRUCTIONS.md_working_4.datopes" onclick='showPath("INSTRUCTIONS.md_working_4.dat","INSTRUCTIONS.md_working_4.datopes","INSTRUCTIONS.md_working_4.datopes","black")'>opes</b><span style="display:none;" id="INSTRUCTIONS.md_working_4.datopes">The OPES_METAD action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">opes.rct</td><td width="5%"><font color="black">scalar</font></td><td>estimate of c(t). log(exp(beta V)/beta, should become flat as the simulation converges. Do NOT use for reweighting</td></tr><tr><td width="5%">opes.zed</td><td width="5%"><font color="black">scalar</font></td><td>estimate of Z_n. should become flat once no new CV-space region is explored</td></tr><tr><td width="5%">opes.neff</td><td width="5%"><font color="black">scalar</font></td><td>effective sample size</td></tr><tr><td width="5%">opes.nker</td><td width="5%"><font color="black">scalar</font></td><td>total number of compressed kernels used to represent the bias</td></tr></table></span>: <div class="tooltip" style="color:green">OPES_METAD<div class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_4.datdefopes");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalars on which the bias will act<i></i></div></div>=<b name="INSTRUCTIONS.md_working_4.datphi">phi</b>,<b name="INSTRUCTIONS.md_working_4.datpsi">psi</b> <div class="tooltip">PACE<div class="right">the frequency for kernel deposition<i></i></div></div>=500 <div class="tooltip">BARRIER<div class="right">the free energy barrier to be overcome<i></i></div></div>=40
</span><span id="INSTRUCTIONS.md_working_4.datdefopes_long" style="display:none;"><b name="INSTRUCTIONS.md_working_4.datopes" onclick='showPath("INSTRUCTIONS.md_working_4.dat","INSTRUCTIONS.md_working_4.datopes","INSTRUCTIONS.md_working_4.datopes","black")'>opes</b>: <div class="tooltip" style="color:green">OPES_METAD<div class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_4.datdefopes");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalars on which the bias will act<i></i></div></div>=<b name="INSTRUCTIONS.md_working_4.datphi">phi</b>,<b name="INSTRUCTIONS.md_working_4.datpsi">psi</b> <div class="tooltip">PACE<div class="right">the frequency for kernel deposition<i></i></div></div>=500 <div class="tooltip">BARRIER<div class="right">the free energy barrier to be overcome<i></i></div></div>=40  <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=-1 <div class="tooltip">SIGMA<div class="right"> the initial widths of the kernels<i></i></div></div>=ADAPTIVE <div class="tooltip">COMPRESSION_THRESHOLD<div class="right"> merge kernels if closer than this threshold, in units of sigma<i></i></div></div>=1 <div class="tooltip">FILE<div class="right"> a file in which the list of all deposited kernels is stored<i></i></div></div>=KERNELS
</span></pre>
 {% endraw %} 

This example gives us a nice opportunity to visualize the kernel compression algorithm in action.
We can also get an idea of the differences between [OPES_METAD](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html) and [OPES_METAD_EXPLORE](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d__e_x_p_l_o_r_e.html) methods.
The plumed inputs are identical:

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_INSTRUCTIONS.md_working_5.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="INSTRUCTIONS.md_working_5.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="INSTRUCTIONS.md_working_5.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="INSTRUCTIONS.md_working_5.datphi" onclick='showPath("INSTRUCTIONS.md_working_5.dat","INSTRUCTIONS.md_working_5.datphi","INSTRUCTIONS.md_working_5.datphi","black")'>phi</b><span style="display:none;" id="INSTRUCTIONS.md_working_5.datphi">The TORSION action with label <b>phi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">phi</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=5,7,9,15
<b name="INSTRUCTIONS.md_working_5.datpsi" onclick='showPath("INSTRUCTIONS.md_working_5.dat","INSTRUCTIONS.md_working_5.datpsi","INSTRUCTIONS.md_working_5.datpsi","black")'>psi</b><span style="display:none;" id="INSTRUCTIONS.md_working_5.datpsi">The TORSION action with label <b>psi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">psi</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=7,9,15,17
<span id="INSTRUCTIONS.md_working_5.datdefopes_short"><b name="INSTRUCTIONS.md_working_5.datopes" onclick='showPath("INSTRUCTIONS.md_working_5.dat","INSTRUCTIONS.md_working_5.datopes","INSTRUCTIONS.md_working_5.datopes","black")'>opes</b><span style="display:none;" id="INSTRUCTIONS.md_working_5.datopes">The OPES_METAD_EXPLORE action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">opes.rct</td><td width="5%"><font color="black">scalar</font></td><td>estimate of c(t). log(exp(beta V)/beta, should become flat as the simulation converges. Do NOT use for reweighting</td></tr><tr><td width="5%">opes.zed</td><td width="5%"><font color="black">scalar</font></td><td>estimate of Z_n. should become flat once no new CV-space region is explored</td></tr><tr><td width="5%">opes.neff</td><td width="5%"><font color="black">scalar</font></td><td>effective sample size</td></tr><tr><td width="5%">opes.nker</td><td width="5%"><font color="black">scalar</font></td><td>total number of compressed kernels used to represent the bias</td></tr></table></span>: <div class="tooltip" style="color:green">OPES_METAD_EXPLORE<div class="right">On-the-fly probability enhanced sampling with well-tempered target distribution in exploreation mode. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_5.datdefopes");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d__e_x_p_l_o_r_e.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalars on which the bias will act<i></i></div></div>=<b name="INSTRUCTIONS.md_working_5.datphi">phi</b>,<b name="INSTRUCTIONS.md_working_5.datpsi">psi</b> <div class="tooltip">PACE<div class="right">the frequency for kernel deposition<i></i></div></div>=500 <div class="tooltip">BARRIER<div class="right">the free energy barrier to be overcome<i></i></div></div>=40
</span><span id="INSTRUCTIONS.md_working_5.datdefopes_long" style="display:none;"><b name="INSTRUCTIONS.md_working_5.datopes" onclick='showPath("INSTRUCTIONS.md_working_5.dat","INSTRUCTIONS.md_working_5.datopes","INSTRUCTIONS.md_working_5.datopes","black")'>opes</b>: <div class="tooltip" style="color:green">OPES_METAD_EXPLORE<div class="right">On-the-fly probability enhanced sampling with well-tempered target distribution in exploreation mode. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("INSTRUCTIONS.md_working_5.datdefopes");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d__e_x_p_l_o_r_e.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the labels of the scalars on which the bias will act<i></i></div></div>=<b name="INSTRUCTIONS.md_working_5.datphi">phi</b>,<b name="INSTRUCTIONS.md_working_5.datpsi">psi</b> <div class="tooltip">PACE<div class="right">the frequency for kernel deposition<i></i></div></div>=500 <div class="tooltip">BARRIER<div class="right">the free energy barrier to be overcome<i></i></div></div>=40  <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=-1 <div class="tooltip">SIGMA<div class="right"> the initial widths of the kernels, divided by the square root of gamma<i></i></div></div>=ADAPTIVE <div class="tooltip">COMPRESSION_THRESHOLD<div class="right"> merge kernels if closer than this threshold, in units of sigma<i></i></div></div>=1 <div class="tooltip">FILE<div class="right"> a file in which the list of all deposited kernels is stored<i></i></div></div>=KERNELS
</span></pre>
 {% endraw %} 

From here it should be easy to compare both OPES variants to metadynamics, maybe by running some longer simulations.
We can also check the way the bias converges by focusing on the estimate of the free energy difference between the basins.

### Biasing more CVs: alanine tetrapeptide

In order to experiment with more than two CVs, we have to introduce a new system, alanine tetrapeptide in vacuum (ala4).
It is a bigger brother of ala2, with not one but three $\phi$ and $\psi$ torsional angles, that can be used to sample its 8 metastable basins.

We can try to sample ala4 with each of the tree methods, [METAD](https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html), [OPES_METAD](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html), and [OPES_METAD_EXPLORE](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d__e_x_p_l_o_r_e.html).
How will the respective input files look like?

We run only short simulations to see how quickly the CV space is sampled by the various methods, and not for converging a FES.
This example can help to appreciate the effect of the $Z$ term in [OPES_METAD](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html).
In fact, the more CVs there are, the more it plays an important role in speeding up exploration.

We can also see the effect of changing the bias factor $\gamma$ on the sampling efficiency.


### 2.4 Biasing a suboptimal CV

Finally, what is probably the most interesting scenario.
We bias again ala2, but this time using a suboptimal collective variable.
We don't know much about this CV, it could be for instance the output of a machine learning procedure.
Will we be able to calculate the FES as a function of this CV? How should the plumed input files look like?
Here it would be nice to also have some error bars to our estimates.

We will discuss together the results of these simulations, and also reveal how this CV was constructed.

If you prefer a more straightforward example of suboptimal CV, you can check out this other [OPES_METAD tutorial](https://www.plumed.org/doc-master/user-doc/html/opes-metad.html).

## Conclusion

Hopefully this masterclass helped you to start playing around with the OPES method and get a sense of what it can be useful for.
If you are still interested in testing it out and understanding more about it, then you should check out the [PLUMED-NEST](https://www.plumed-nest.org/browse.html).
Just search for "opes" and you will find several papers that use the method, together with all the input files necessary to reproduce their simulations.

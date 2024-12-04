<div align="center">
<img src="https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/blob/main/images/LIFDlogo.png"></a>
<a href="https://www.cemac.leeds.ac.uk/">
  <img src="https://github.com/cemac/cemac_generic/blob/master/Images/cemac.png"></a>
  <br>
</div>

# Leeds Institute for Fluid Dynamics Machine Learning For Earth Sciences

# Design Optimisation with Metamodels

[![GitHub release](https://img.shields.io/github/release/cemac/LIFD_DesignOptimisation.svg)](https://github.com/cemac/LIFD_DesignOptimisation/releases) [![GitHub top language](https://img.shields.io/github/languages/top/cemac/LIFD_DesignOptimisation.svg)](https://github.com/cemac/LIFD_DesignOptimisation) [![GitHub issues](https://img.shields.io/github/issues/cemac/LIFD_DesignOptimisation.svg)](https://github.com/cemac/LIFD_DesignOptimisation/issues) [![GitHub last commit](https://img.shields.io/github/last-commit/cemac/LIFD_DesignOptimisation.svg)](https://github.com/cemac/LIFD_DesignOptimisation/commits/main) [![GitHub All Releases](https://img.shields.io/github/downloads/cemac/LIFD_DesignOptimisation/total.svg)](https://github.com/cemac/LIFD_DesignOptimisation/releases) ![GitHub](https://img.shields.io/github/license/cemac/LIFD_DimensionalityReduction.svg) [![DOI](https://zenodo.org/badge/366734586.svg)](https://zenodo.org/badge/latestdoi/366734586)

[![LIFD_ENV_ML_NOTEBOOKS](https://github.com/cemac/LIFD_DesignOptimisation/actions/workflows/python-package-conda-unet.yml/badge.svg)](https://github.com/cemac/LIFD_DesignOptimisation/actions/workflows/python-package-conda-unet.yml)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cemac/LIFD_DesignOptimisation/HEAD?labpath=Design_Optimisation_Metamodels.ipynb)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cemac/LIFD_DesignOptimisation/blob/main/Design_Optimisation_Metamodels.ipynb)

This Jupyter notebook demonstrates how machine-learning metamodels can be used to solve fluid mechanical design optimisation problems. Here, design optimisation refers to the process of finding the best solution to an engineering problem within constraints using mathematical techniques. Metamodels allow us to explore parameter space to find optimal solutions to Partial Differential Equations (PDEs) while only running a relatively small number of costly Computational Fluid Dynamics (CFD) simulations. This notebook contains an example application to coronary bypass anastomosis, a surgical procedure used to treat coronary artery disease ([Lassila et al., 2013](https://doi.org/10.1051/m2an/2012059)).

## Quick look

### Quick start

**Binder and Colab buttons**

Will launch this tutorial in binder or Google Colab.

**Running locally**

If you're already familiar with Git, Anaconda and virtual environments, the environment you need to create is found in [DO.yml](https://github.com/cemac/LIFD_DesignOptimisation/blob/main/DO.yml) and the code below will install, activate and launch the notebook. The .yml file has been tested on the latest Linux, macOS and Windows operating systems.

```bash
git clone git@github.com:cemac/LIFD_DesignOptimisation.git
cd LIFD_DesignOptimisation
conda env create -f DO.yml
conda activate DO
jupyter-notebook
```

## Installation and requirements

This notebook is designed to run on a laptop with no special hardware required. However, training of neural networks can take a long time (hours) without dedicated GPU hardware. If you have a GPU, it is recommended to do a local installation as outlined in the repository [howtorun](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/howtorun.md) and [jupyter_notebooks](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS/jupyter_notebooks.md) sections. Otherwise, online compute platforms which offer GPU access (e.g. Google Colab) are strongly recommended.

## Licence Information

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">LIFD_ENV_ML_NOTEBOOKS</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://cemac.leeds.ac.uk/" property="cc:attributionName" rel="cc:attributionURL">CEMAC</a> are licenced under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

## Acknowledgements

Thanks to Toni Lassila for providing code and material for this notebook. This tutorial is part of the [LIFD_ENV_ML_NOTEBOOKS](https://github.com/cemac/LIFD_ENV_ML_NOTEBOOKS) series. Please refer to the parent repository for full acknowledgements.

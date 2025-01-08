<img src="notebooks/images/logos/esgf2-us.png" alt="thumbnail" width="300"/>

# ESGF Cookbook

[![nightly-build](https://github.com/ProjectPythia/esgf-cookbook/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/esgf-cookbook/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/esgf-cookbook/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/721319801.svg)](https://doi.org/10.5281/zenodo.11663067)

This Project Pythia Cookbook covers how to access and analyze datasets that can be accessed from Earth System Grid Federation (ESGF) cyberinfrastructure.

## Motivation

This cookbook focuses on highlighting analysis recipes, as well as data acccess methods, all accesible within the Python programming language. This cookbook also spans beyond the scope of a single Climate Model Intercomparison Project (ex. CMIP6), expanding to other experiments/datasets such as CMIP5 and obs4MIPs.

## Authors

[Max Grover](@mgrover1), [Nathan Collier](@nocollier), [Carsten Ehbrecht](@cehbrecht), [Jacqueline Nugent](@jacnugent), [Gerardo Rivera Tello](@griverat)

### Contributors

<a href="https://github.com/ProjectPythia/esgf-cookbook/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/esgf-cookbook" />
</a>

## Structure

### Searching

This content includes details on how to search for datasets hosted on ESGF cyberinfrastructure.

### Workflows

Scientific workflows utilizing data accessed from ESGF.

## Running the Notebooks

You can either run the notebook using [the NIMBUS Juptyerhub](https://nimbus.llnl.gov) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[the NIMBUS Juptyerhub](https://nimbus.llnl.gov), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) in the cloud-like infrastructure. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Cookbooks chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter.html).

### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

(Replace "cookbook-example" with the title of your cookbooks)

1. Clone the `https://github.com/esgf2-us/esgf-cookbook` repository:

   ```bash
    git clone https://github.com/esgf2-us/esgf-cookbook.git
   ```

1. Move into the `cookbook-example` directory
   ```bash
   cd esgf-cookbook
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate esgf-cookbook-dev
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```

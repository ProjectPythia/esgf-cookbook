# Running Notebooks on Nimbus

Interested in running your notebooks on ESGF infrastructure? Please follow these steps!

## 1. Apply for access to the Nimbus Access

Please fill out [this form](https://forms.gle/h8y14hfefcaCraEJ8) to request access to the Nimbus Jupyterhub!

You will be added to the [Nimbus User Group](https://github.com/orgs/esgf-nimbus/people), which is used for authentication!

## 2. Clone this repository

Once you log into the Jupyterhub (https://nimbus.llnl.gov/), go to your home directory (shown by default) and clone this repository

```bash
git clone https://github.com/ProjectPythia/esgf-cookbook.git
```

## 3. Build your Execution Environment
The cookbook environment is slightly different than the base environment available on the hub. You will need to build the required environment, using the `environment.yml` file in the repository.

```bash
conda env create -f esgf-cookbook/environment.yml
```

## Activate Your Environment
Once you build the enivronment, you will need to activate it. You will need to follow the following steps:

```bash
# Make sure you can activate the environment
source .bashrc

# Activate the environment
conda activate esgf-cookbook-dev
```

## Open a Notebook and Select the `esgf-cookbook-dev` environment
Now that you have an environment, you can select this when opening a notebook. Select in the top right corner the kernel options, and select `esgf-cookbook-dev`.

Wait a second for the notebook to pick up on this, then execute your cells!

If you need to install more packages, or update versions, you can do so by updating your `environment.yml` file or by installing via the command line. 
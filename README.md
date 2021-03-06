# Anaconda Environments

This repository contains YAML files of useful anaconda environments. These environments are loaded and automatically installed by containers such as [Ubuntu-Python-Dev-Env](https://hub.docker.com/r/andrewhills/ubuntu-python-dev-env). 

## Manual Environment Creation

**Note: For up-to-date information on manually creating an environment from an `environment.yml` file, please check the [official Anaconda documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file).**

At the time of writing, to create an environment from the file `environment.yml` (replacing the filename with the environment file of your choice), run from the Terminal/Command Prompt/PowerShell:

  ```bash
  conda env create -f environment.yml
  ```

To activate an environment, type in the following into the Terminal/Command Prompt/PowerShell:

  ```bash
  conda activate myenv
  ```

where `myenv` is the name of the environment listed below. In some instances, it is necessary to use the command `source activate myenv` instead.

To ensure an environment has been installed correctly, type in the following command into the Terminal/Command Prompt/PowerShell:

  ```bash
  conda list
  ```

This command will return a list of the installed environments.  

## Description of Environments

This section contains a list of the environments, the name to activate it within `conda` and their contents.

### Python 3 Latest (`py3_latest`)

Environment with latest Python 3 version including basic data science tools such as `scipy`, `sklearn` and `pandas` as well as `cython` for compiling shared libraries. Use:

`conda activate py3_latest`

### Python 3.6 (`py3_6`)

Copy of `py3_latest` but with Python version forced to 3.6 for compatibility with legacy systems. Use:

`conda activate py3_6`

### Python 2 Latest (`py2_latest`)

Copy of `py3_latest` but with the latest version of Python 2. Use:

`conda activate py2_latest`

### Data Science  (`data_science`)

Extension of `py3_latest` environment with more advanced tools including `statsmodels` and `keras`. This environment was separated to avoid bloating `py3_latest`.
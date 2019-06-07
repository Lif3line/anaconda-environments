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

### Python 3 Latest

Latest Python 3 version with basic data science tools such as `scipy`, `sklearn` and `pandas` as well as `cython` for compiling shared libraries. Use:

`conda activate py3_latest`

Weeks 1&2
[RUG-Elective/Notebooks](https://mybinder.org/v2/gh/RUG-Elective/Notebooks_official/df013bd08f17b7e8f89b46bf6082e97aa1185bde?urlpath=lab%2Ftree%2FWeek_1_2%2FSection%201.ipynb)

# Using mamba to create the Geo-Python environment

## Starting steps
This briefly describes how to install a Python virtual environment for the Geo-Python course.

1. Install miniconda from https://docs.conda.io/en/latest/miniconda.html
2. Install mamba
    ```bash
    conda install mamba -n base -c conda-forge
    ```
3. Clone the course Python environments from GitHub
    ```bash
    git clone https://github.com/geo-python/python-environments.git
    ```
4. Change into the working directory with the cloned environment files
    ```bash
    cd python-environments
    ```
## Creating the environment for students
1. Create the python environment using mamba
    ```bash
    mamba env create -f geo-python-student.yml
    ```
2. Activate the new environment and update JupyterLab
    ```bash
    conda activate geo-python-student
    sh postBuild
    ```
## Creating the environment for teachers
1. Create the python environment using mamba
    ```bash
    mamba env create -f geo-python-teacher.yml
    ```
2. Activate the new environment and update JupyterLab
    ```bash
    conda activate geo-python-teacher
    sh postBuild
    ```




## Follow the course through Binder: Weeks 1&2
[RUG-Elective/Notebooks](https://mybinder.org/v2/gh/RUG-Elective/Notebooks_official/main?labpath=Weeks_1_2.ipynb)

## Using mamba to create the Geo-Python environment

## Starting steps
This briefly describes how to install a Python virtual environment for the Geospatial course.

1. Install miniconda from https://docs.conda.io/en/latest/miniconda.html
2. Install mamba
    ```bash
    conda install mamba -n base -c conda-forge
    ```
3. Clone the course from GitHub
    ```bash
    https://github.com/RUG-Elective/Notebooks_official.git
    ```
4. Change into the working directory with the cloned environment file (yml)
    ```bash
    cd python-environments
    ```
## Creating the environment for students
1. Create the python environment using mamba
    ```bash
    mamba env create -f geospatial-student.yml
    ```
2. Activate the new environment
    ```bash
    conda activate geospatial-student
    ```
3. Install JupyterLab
   ```bash
   pip install jupyterlab
   ```
4. Install a new kernel (ipykernel) for the virtual environment
   ```bash
   pip install ipykernel
   ```
5. Register the environment as a kernel, give it a name and a display name
   ```bash
   python -m ipykernel install --user --name geospatial-student --display-name "Python (geospatial-student)"
   ```
6. Run Jupyterlab
   ```bash
   jupyter lab
  ```

# ROOT LHCb Open Data Analysis

This repository contains an example analysis of LHCb open data from the University of Manchester undergraduate laboratory project on matter-antimatter asymmetries. 
Here we demonstrate an alternative implementation of the solution rewritten with ROOT.

## Setup
- Download the prerequisite root files into the `data/` folder using `download.sh`: `chmod +x download.sh && ./download.sh`
- If using `conda`:
    - Create a conda environment for this project: `conda env create -f environment.yml`
    - Activate the newly created environment: `conda activate lhcb_open_analysis`
    - Register the environment as a Jupyter kernel: `python -m ipykernel install --user --name lhcb_open_analysis`
- If using `pip`:
    - Create a virtual environment for this project: `python -m venv .venv`
    - Source the venv: `source .venv/bin/activate`
    - Install dependencies: `pip install -r requirements.txt`
    - Register the venv as a Jupyer kernel: `python -m ipykernel install --user --name lhcb_open_analysis`
- If using `uv`, follow the `pip` instructions but create the venv with `uv venv` and run `pip` via `uv pip`

## Structure

- `original_solution/`  
  Contains the original analysis solution notebook provided by the lab.

- `rdf_solution/`  
  Contains a notebook implementing the analysis using ROOT RDataFrame.

- `distrdf_solution/`  
  Contains a notebook implementing the analysis using ROOT distributed RDataFrame using a Dask Client.

- `data/`  
  Download the input data and place it in this folder.
  Input data files can be downloaded from the original repository:  
  [UoM_MatterAntimatterLab/postBuild](https://github.com/gersabec/UoM_MatterAntimatterLab/blob/master/postBuild)

- `outputs/`  
  Folder to store generated histograms and plots.

- `benchmarks/`  
  Folder to store results of performance comparison between the original analysis and the RDataFrame based analysis.
  
## Original repository

This project is based on the original University of Manchester lab:  
[https://github.com/gersabec/UoM_MatterAntimatterLab](https://github.com/gersabec/UoM_MatterAntimatterLab)

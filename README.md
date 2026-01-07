# ROOT LHCb Open Data Analysis

This repository contains an example analysis of LHCb open data from the University of Manchester undergraduate laboratory project on matter-antimatter asymmetries. 
Here we demonstrate an alternative implementation of the solution rewritten with ROOT.

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

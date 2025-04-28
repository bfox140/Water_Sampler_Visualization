# Water Sampler Visualization

This repository contains a Jupyter Notebook, dataset, and environment file related to the analysis of chlorophyll concentrations collected using a novel autonomous water sampling mechanism.  
The project compares chlorophyll levels between control samples (collected manually) and experimental samples (collected with the new sampler) at two locations: a pond and the Raritan River.

## Files

- `chlorophyll_plot.ipynb` — Jupyter Notebook for generating violin plots comparing chlorophyll concentrations
- `Chlorophyll Template Generic_Bodhi.csv` — Input CSV file with chlorophyll concentration data
- `environment.yml` — Conda environment file to recreate the exact software setup
- `README.md` — Project description and setup instructions

## Data Description

The data (`Chlorophyll Template Generic_Bodhi.csv`) was collected during field testing at Rutgers University's Passion Puddle and the Raritan River.  
Water samples were taken using two methods: manual bottle sampling (control) and the Remora autonomous sampling mechanism (experimental).  
Chlorophyll concentrations were measured fluorometrically to compare the performance of the two sampling approaches.  
All data was personally collected; no external datasets were used.

## Environment Setup

To recreate the environment:

```bash
conda env create -f environment.yml
conda activate chlorophyll_env

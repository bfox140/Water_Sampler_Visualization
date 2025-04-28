# Water Sampler Visualization

This repository contains a Jupyter Notebook, dataset, and environment file related to the analysis of chlorophyll concentrations collected using a novel autonomous water sampling mechanism.  
The project compares chlorophyll levels between control samples (collected manually) and experimental samples (collected with the new sampler) at two locations: a pond and the Raritan River.

## Files

- `Thesis_Chla_Analysis.ipynb` — Jupyter Notebook for generating violin plots comparing chlorophyll concentrations
- `Chlorophyll Template Generic_Bodhi.csv` — Input CSV file with chlorophyll concentration data
- `environment.yml` — Conda environment file to recreate the exact software setup
- `README.md` — Project description and setup instructions

## Data Description

The data (`Chlorophyll Template Generic_Bodhi.csv`) was collected during field testing at Rutgers University's Passion Puddle and the Raritan River.  
Water samples were taken using two methods: manual bottle sampling (control) and the novel sampling mechanism (experimental).  
Chlorophyll concentrations were measured fluorometrically to compare the performance of the two sampling approaches.  
All data was personally collected; no external datasets were used.

## Environment Setup

To recreate the environment:

```bash
conda env create -f environment.yml
conda activate chlorophyll_env
```

## Usage Instructions

1. Clone or download this repository.
2. Activate the environment (`chlorophyll_env`) or ensure required packages are installed.
3. Launch Jupyter Notebook or JupyterLab:
4. Run all cells in the notebook.
5. The resulting violin plots will compare chlorophyll concentrations across sites and sampling methods.  
6. The plot will be saved automatically as `chlorophyll_violinplot.png` in the working directory.

## Project Summary

This repository supports the research project focused on designing and validating a low-cost, modular water sampling mechanism for autonomous surface vehicles (ASVs) like the WasteShark made by RanMarine Technologies.  
The water sampler, adapted from the open-source Niskin3D design, was tested for mechanical efficiency and performance in collecting biological water quality parameters.  
Specifically, chlorophyll concentrations were used as a key indicator to assess whether the sampler produced comparable results to traditional manual methods.

Results indicated that the novel sampler achieved an average sampling efficiency of 98.7% with a 10% misfire rate.  
Preliminary field testing showed that chlorophyll concentrations collected using the sampler were broadly consistent with those obtained through manual sampling, with differences between methods around 5 µg/L.  
Although the sample size was small, these results demonstrate the potential for low-cost autonomous water samplers to enable wider environmental monitoring without significant loss of data quality.

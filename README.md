# Water_Sampler_Visualization
This repository contains a Jupyter Notebook and associated files for visualizing chlorophyll concentrations collected during field sampling.  
The project compares chlorophyll levels between control and experimental groups at two locations: a pond and the Raritan River.

## Files
- `chlorophyll_plot.ipynb` — Jupyter Notebook for generating violin plots
- `Chlorophyll Template Generic_Bodhi.csv` — Input CSV file with chlorophyll data
- `environment.yml` — Conda environment file to recreate the exact software setup
- `README.md` — Project description and setup instructions

## Environment Setup

The environment for this project is provided in `environment.yml`.  
To recreate the environment:

```bash
conda env create -f environment.yml
conda activate [your-environment-name]

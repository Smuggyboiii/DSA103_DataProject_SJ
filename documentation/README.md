# DSA103 Data Project — Leaf Metabolite AnalysisAuthor: Julian Patrick Stoerr

Date 01.12.2025
Course: DSA103 (UZH, HS25)

This repository contains a Python-based re-analysis of plant metabolite data from Walker et al. (2023).
The goal of this project is to explore whether chemical descriptors extracted from metabolite structures reveal interpretable and clear structure in their molecular profiles using unsupervised learning and dimensionality reduction.

## Project Structure

├── data/ # Data files (not included in repository)  
├── documentation/ # Written reports and documentation  
│ ├── Documentation and Data Management Plan.docx  
│ └── DSA103 Data Project.docx  
├── modified_data/ # Processed / intermediate data (local only)  
├── scripts/ # Analysis notebooks and scripts  
│ └── derive_chemistry.ipynb  
├── .gitignore # Excludes large data files  
└── README.md

## Data Availability

Raw data are excluded from this repository due to size constraint and can be found on `Dryad: https://datadryad.org/dataset/doi:10.5061/dryad.zpc866tdn`

## Workflow

The workflow includes
- Filtering metabolites with valid SMILES Code
- Chemical descriptor from SMILES using RDKit
- Dimensionality Reduction using PCA
- KMeans Clustering with silhouette-analysis
- Correlation analysis and heatmap visualisation

### Requirements

- Python 3.9+
- Required libraries
	- pandas
	- scikit-learn
	- seaborn
	- matplotlib
	- RDKit

### References

- Walker et al. (2023), *Leaf metabolic traits reveal hidden dimensions of plant form and function.*, https://doi.org/10.1101/2023.03.08.531692

### Reproducibility

- All data transformations and analysis are fully scripted and complete. 
- No raw data files are modified
- All results can be reproduced by running the notebook from top to bottom

### License and Usage

This repository is for education and research purposes only and only uses publicly available data and code packages.
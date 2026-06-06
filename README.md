
# AIDD_Demo

Minimal demo for AI-assisted Drug Discovery (AIDD):  
molecule parsing → drug-likeness (Lipinski) filtering → molecular fingerprint extraction → machine learning-based activity prediction.

## Contents

- `AIDD_Molecule_Demo.ipynb` — Jupyter Notebook implementing the full AIDD pipeline  
- `molecules.csv` — Sample SMILES dataset with binary activity labels  
- `requirements.txt` — Python dependencies

## Pipeline Overview

1. Load SMILES and validate molecules with **RDKit**
2. Apply **Lipinski Rule-of-Five** drug-likeness filter
3. Compute **Morgan Fingerprints (ECFP)** as molecular features
4. Train a **Random Forest classifier** to predict bioactivity
5. Evaluate with ROC-AUC and visualize feature importance

## Usage

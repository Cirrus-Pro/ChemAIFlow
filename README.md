# ChemAIFlow: A Lightweight AI Workflow for Protein–Ligand Binding Analysis

## Overview
ChemAIFlow is a lightweight, reproducible Wolfram Language workflow designed for protein–ligand binding affinity modelling.  
It supports both **online** and **offline** installation modes and automatically generates working directories containing runnable workflow notebooks.

This repository accompanies the software submission to the *Journal of Statistical Software (JSS)*.

---

## Features
- Online and offline installation options  
- Automatic folder generation after installation  
- Reproducible descriptor engineering and modelling pipeline  
- Lightweight operation suitable for constrained hardware environments  
- Includes main workflows:  
  - `ChemAIFlow_Main_Online.nb`  
  - `ChemAIFlow_Main_Offline.nb`  

---

## Repository Structure

```
ChemAIFlow/
│
├── install/
│     ├── Install_v1.0.0_Online.nb
│     ├── Install_v1.0.0_Offline.nb
│
├── data/
│     ├── Protein_Ligand_AllFeatures_NoOutlier_Dedup.wl
│
└── README.md
```

After installation (online or offline), the installer automatically creates:

```
ChemAIFlow/
│
└── Workflows/
      ├── ChemAIFlow_Main_Online.nb
      └── ChemAIFlow_Main_Offline.nb
```

---

## Installation Guide

### 🔹 Online Installation
1. Download `Install_v1.0.0_Online.nb`
2. Place any dataset file (`Protein_Ligand_AllFeatures_NoOutlier_Dedup.wl`, if used) **in the same folder** as the installer.
3. Open the installer in Wolfram Mathematica.
4. Run all cells.  
   The program will create the `Workflows/` directory and generate:
   - `ChemAIFlow_Main_Online.nb`

---

### 🔹 Offline Installation
Required files:
- `Install_v1.0.0_Offline.nb`  
- `Protein_Ligand_AllFeatures_NoOutlier_Dedup.zip` → extract → `Protein_Ligand_AllFeatures_NoOutlier_Dedup.wl`

Steps:
1. Extract the `.zip` file.  
2. Place `Protein_Ligand_AllFeatures_NoOutlier_Dedup.wl` **in the same folder** as the offline installer.  
3. Open `Install_v1.0.0_Offline.nb`  
4. Run all cells.  
   The installer will import the dataset and create:
   - `ChemAIFlow/Workflows/ChemAIFlow_Main_Offline.nb`

---

## Dataset Description
**Protein_Ligand_AllFeatures_NoOutlier_Dedup.wl** contains preprocessed, deduplicated descriptors used for model training.  
When placed beside an installer notebook, the installation script automatically imports and relocates it into the appropriate internal directory.

---

## Usage
After installation:

1. Open the `Workflows/` folder.
2. Choose either:
   - `ChemAIFlow_Main_Online.nb`
   - `ChemAIFlow_Main_Offline.nb`
3. Run the notebook to begin descriptor processing, model training, and evaluation.

---

## Citation

If using ChemAIFlow in scientific work, please cite:

```
Yaiprasert, C. (2025).
ChemAIFlow: A Lightweight and Reproducible AI Workflow for Protein–Ligand Binding Affinity Prediction.
Journal of Statistical Software. (Submitted)
```

---

## Contact
**Chairote Yaiprasert**  
School of Science, Walailak University  
Email: ychairot@mail.wu.ac.th

---

## License
This project is released under the GNU General Public License (GPL) v3.

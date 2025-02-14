# CT Scan Analysis

## Overview
This project is designed for the analysis of **CT scan images**, specifically focusing on **airway segmentation** and **blockage quantification**. The analysis includes:
- **Loading and visualizing DICOM images**
- **Segmenting airways based on Hounsfield Units (HU)**
- **Measuring airway volume and cross-sectional area**
- **Detecting potential airway obstructions**
- **3D visualization of airway structures**

## Directory Structure
```
ct_scan/
├── raw_data/              # Stores raw DICOM files (ignored by .gitignore)
│   ├── dicom/             # Subdirectory for DICOM images
│   ├── metadata/          # Stores extracted metadata from DICOM files
│   └── uploads/           # Temporary directory for uploaded files
├── analysis/              # Jupyter notebooks and scripts for processing
│   ├── 01_preprocessing.ipynb  # Load and preprocess DICOM images
│   ├── 02_segmentation.ipynb   # Segment airways
│   ├── 03_visualization.ipynb  # 3D rendering and volume calculations
│   ├── 04_quantification.ipynb # Airway blockage analysis
│   └── utils/                  # Helper scripts for processing
├── results/               # Processed data and analysis results
│   ├── plots/             # Figures and visualizations
│   ├── volumes/           # Computed airway volume data
│   └── annotations/       # CSV files with extracted metadata or results
├── environment.yml        # Conda environment definition
├── LICENSE                # Project license (BSD-3-Clause)
├── README.md              # Project overview and usage instructions
└── .gitignore             # Files and directories to ignore in version control
```

## Installation
### **1. Create the Conda Environment**
Run the following to set up the environment:
```sh
conda env create -f environment.yml
conda activate ct_analysis
```

### **2. Install Jupyter Kernel (if not installed)**
```sh
python -m ipykernel install --user --name=ct_analysis
```

## Usage
### **1. Run Jupyter Lab**
```sh
jupyter lab
```

### **2. Open Notebooks**
- `01_preprocessing.ipynb` → Load and explore CT scan images
- `02_segmentation.ipynb` → Segment airways
- `03_visualization.ipynb` → Generate 3D airway models
- `04_quantification.ipynb` → Analyze airway obstruction

## Contribution
If you'd like to contribute, fork the repository, create a feature branch, and submit a pull request.

## License
This project is licensed under the **BSD-3-Clause License**.

## Contact
**Sebastian Eguiguren**  
Email: sebastian.eguiguren@tu-dresden.de  
GitHub: [jseguiguren](https://github.com/jseguiguren)


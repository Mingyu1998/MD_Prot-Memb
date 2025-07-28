# 🧬 MD_Prot-Memb Analysis Toolkit

![MDAnalysis](https://img.shields.io/badge/Powered%20by-MDAnalysis-orange.svg)
![Python Version](https://img.shields.io/badge/Python-3.9+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

This repository contains a collection of Python scripts for analyzing molecular dynamics (MD) simulations of protein-membrane systems. The tools are written to work with the **MDAnalysis** library and are primarily designed for Coarse-Grained (CG) simulation data.

This toolkit was developed as part of a DPhil project in Computational Biochemistry, focusing on the interactions between PAMAM dendrimers and bacterial membrane models.

## 🔬 Key Analyses Included

This collection provides functions to perform a wide range of common and advanced membrane analyses:

* **2D Density Maps**: Calculate spatial density maps for lipids or other molecules in the X-Y or X-Z planes.
* **Leaflet Identification**: Includes two robust methods for assigning lipids to leaflets:
    * A fast, Z-coordinate-based midplane method.
    * An advanced **DBSCAN clustering** method for curved or disrupted membranes.
* **Membrane Thickness & Curvature**:
    * `calculate_membrane_thickness`: Uses Radial Basis Functions (RBF) to create a smooth surface map of local membrane thickness.
    * `calculate_mean_curvature`: Computes the mean curvature (H) across the membrane surface.
* **Lipid Order & Dynamics**:
    * `calculate_scd_profile`: Calculates deuterium order parameters ($S_{CD}$) for various Martini lipids from a built-in library.
    * `calculate_lipid_tilt_angle`: Tracks the orientation of a single lipid throughout a trajectory, useful for analyzing flipping events.
* **Interaction Analysis**:
    * `parallel_contacts_within_cutoff`: A highly efficient, parallelized function to calculate the number of contacts between two molecular groups over time.

## ⚙️ Installation & Dependencies

To use these scripts, you will need a Python environment with the following major packages installed.

```bash
pip install mdanalysis numpy pandas scikit-learn scipy matplotlib tqdm


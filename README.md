# 🧬 MD_Prot-Memb Analysis Toolkit

![MDAnalysis](https://img.shields.io/badge/Powered%20by-MDAnalysis-orange.svg)
![Python Version](https://img.shields.io/badge/Python-3.9+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

This repository contains a collection of Python scripts for analyzing molecular dynamics (MD) simulations of protein-membrane systems. The tools are written to work with the **MDAnalysis** library and are primarily designed for Coarse-Grained (CG) simulation data.

---

## ✨ Visual Examples

Here are some examples of the plots this toolkit can generate, placed side-by-side for a cleaner look.

| Membrane Properties | Lipid Order Parameters |
| :---: | :---: |
| ![Membrane properties plot](https://github.com/Mingyu1998/MD_Prot-Memb/blob/main/Example_Images/Figure2_IM_split2.png?raw=true) | ![Lipid order parameter plot](https://github.com/Mingyu1998/MD_Prot-Memb/blob/main/Example_Images/OP_para_38_rep3.png?raw=true) |

---

## 🔬 Key Analyses Included

<details>
<summary><b>Click to expand the full list of analysis functions</b></summary>
<br>

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

</details>

---

## ⚙️ Installation & Dependencies

To use these scripts, you will need a Python environment with the following major packages installed.

```bash
pip install mdanalysis numpy pandas scikit-learn scipy matplotlib tqdm


# MD_Prot-Memb

This repository contains a collection of Python scripts for analyzing molecular dynamics (MD) simulations of protein-membrane systems. The tools are written to work with the [MDAnalysis](https://www.mdanalysis.org/) library and are primarily designed for Coarse-Grained (CG) simulation data.

## Implemented Analyses

* **2D Lipid Density:** Calculates 2D number density maps for selected lipid atoms (e.g., headgroups) in different planes.
* **Lipid Order Parameter:** Computes acyl chain order parameters ($S_{CH}$) to describe membrane fluidity, binned into 2D heatmaps.
* **Leaflet Analysis:** Assigns lipids to the upper or lower leaflet using a simple midplane method and tracks population counts over time.
* **Protein-Lipid Interactions:** (You can add more detail here later, e.g., "Monitors contacts and distances between proteins and lipid species.")
* **Membrane Thickness:** (e.g., "Calculates P-P distance maps.")

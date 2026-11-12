# 3I/ATLAS Galactic Backtracking Framework: High-Precision Kinematics and Progenitor System Search via Gaia DR3

[![Python 3.10+](https://shields.io)](https://python.org)
[![ORCID iD](https://shields.io)](https://orcid.org)
[![DOI](https://zenodo.org)](https://doi.org)

[![License: MIT](https://shields.io)](https://opensource.org)

An open-science, high-precision numerical backward-integration framework designed to evaluate the Galactic orbital kinematics and trace the stellar progenitor system of the third interstellar object, **3I/ATLAS**. 

The pipeline couples high-order adaptive numerical integrators (RK45 baseline) with non-gravitational stellar wind outgassing profiles, mapping Galactic trajectories backward in time using astrometric constraints derived from the **Gaia Data Release 3 (DR3)** catalog.

---

## 🛠️ Computational Architecture & Core Dependencies

The pipeline models interstellar kinematics by integrating localized solar barycentric vectors with wide-field Galactic potential models.

### Prerequisites & Libraries
The integration suite compiles custom performance structures and requires the following Python configuration:
* **Mathematical Core:** `numpy`, `scipy` (RK45 adaptive ODE solvers)
* **Astrometry & Ephemerides:** `astropy` (Galactocentric coordinate transformations), `astroquery`
* **Data Ingestion:** Slicing capabilities for local Gaia DR3 stellar kinematics matrices

---

## 📦 Environment Setup

To ensure exact numerical convergence and avoid package conflicts, initialize your local workspace by installing the required dependencies via terminal:

```bash
pip install numpy scipy astropy astroquery matplotlib
```

---

## 🚀 Execution & Pipeline Flow

The backtracking core is structured inside discrete Jupyter Notebook execution cells (`3iatlas_simulation.ipynb`) to secure operational transparency and step-by-step verification:

1. **Cell 1: Ingestion & Ephemerides Bootstrap** -> Loads high-precision state vectors and filters target Gaia DR3 datasets.
2. **Cell 2: Numerical Engine Configuration** -> Sets local tolerances and couples anisotropic solar radiation pressure models.
3. **Cell 3: Backward-Integration Run** -> Runs the adaptive RK45 backward-integration loop into deep Galactic coordinates.
4. **Cell 4: Validation & Boundary Controls** -> Compares results with official baselines and plots parabolic/hyperbolic nodal trajectories.

To run the simulation locally from command-line alternatives:
```bash
python 3iatlas_backtracking.py
```

---


## 📄 Academic Citation

If you use this software simulation framework in your research, please cite it using the Zenodo DOI:

```bibtex
@software{SagalAndrade2026BacktrackingCode,
  author       = {Sagal Andrade, Rene},
  title        = {{3I/ATLAS Galactic Backtracking Framework: High-Precision Kinematics}},
  month        = nov,
  year         = 2026,
  publisher    = {Zenodo},
  version      = {v1.0.2},
  doi          = {10.5281/zenodo.24166495},
  url          = {https://doi.org}
}
```


---

## ✒️ Author & Open-Science Core

* **Rene Sagal Andrade** - *Lead Developer / Computational Astrodynamics Researcher*
* **Verified ORCID iD:** [0009-0003-5574-5384](https://orcid.org)

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

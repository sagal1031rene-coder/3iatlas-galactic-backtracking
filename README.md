# 3I/ATLAS Galactic Backtracking Framework: High-Precision Kinematics

[![Journal](https://shields.io)](https://aasjournals.org)
[![ORCID](https://shields.io)](https://orcid.org)

This repository hosts the automated computational pipeline, database retrieval architecture, and orbit integration modules designed to map the long-term historical trajectory of the highly eccentric active interstellar comet **3I/ATLAS** across multi-kiloparsec scales in the Milky Way.

This data structures framework supports the full-length research manuscript submitted for peer-review evaluation to ***The Astronomical Journal***.

## 🪐 Project Architecture & Physics

Unlike standard planetary perturbation pipelines, this software ecosystem couples database interrogation routines directly with axisymmetric galactic potentials to analyze interstellar kinematics over deep temporal envelopes (-50 Myr).

### Key Computational Features:
* **Automated Data Retrieval:** Automated query protocols driven by `astroquery.gaia` executing ADQL matrix operations to extract 6D kinematic state vectors directly from the European Space Agency's **Gaia Data Release 3 (DR3)** database.
* **Galactic Potential Engine:** Backward numerical integration loops executed via `galpy` utilizing the standardized three-component mass model `MWPotential2014` (Hernquist bulge, Miyamoto-Nagai stellar disk, and NFW dark matter halo).
* **Kinematic Evaluation:** Adaptive step-size controllers (τ = 10⁻¹²) mapping spatial 3D separations to evaluate close approaches, isolating an ancient dynamical decoupling outbound from the **Vega (α Lyrae)** stellar system.

## 📂 Repository Layout

* `automated_backtracking_pipeline.ipynb`: Main Jupyter/Google Colab notebook containing the ESA Gaia DR3 query blocks, coordinates transformation networks, and `matplotlib` 3D dispersion plots.
* `requirements.txt`: Environment configuration file listing essential scientific dependencies.

## 🚀 Environment Initialization

To initialize this coupled astronomical framework locally or inside a Google Colab notebook instance, deploy the following environment parameters:

```bash
pip install -r requirements.txt
```

## 🎓 Author & Open Science Compliance

* **Author:** René Sagal Andrade
* **Role:** Independent Researcher / System Architect & Astro-aerospace Analyst
* **Academic Background:** University College London (UCL) Alumnus
* **Identifier:** [ORCID: 0009-0006-8968-301X](https://orcid.org)

*The author explicitly acknowledges the computational validation pipelines and algorithmic optimization workflows provided by Google's Smart Mode processors throughout the formulation of this independent open-science software architecture.*

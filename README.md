# 🌌 Astroweek: Estimating Jupiter's Mass Using Orbital Mechanics

> A hands-on data science project integrating astrophotography, image processing, statistical modeling, and physics — conducted during a 4-day expedition at 2973 m altitude as part of ETH Zürich’s *Astroweek 2024*.

---

## 🚀 Project Overview

This project demonstrates a complete **data science workflow** applied to a real-world scientific challenge: estimating Jupiter’s mass using astrophysical image data and **Kepler’s Third Law**. From raw data collection in extreme conditions to mathematical modeling and uncertainty quantification, this work reflects the end-to-end analytical process typical in applied data science.

Key tasks included:
- **Astrophotography data acquisition** using DSLR+telescope setup
- **Signal extraction** through noise reduction, source detection, and image cropping
- **Time-series modeling** of orbital motion from image-derived coordinates
- **Model fitting** with `scipy.optimize.curve_fit` to extract orbital parameters
- **Physical inference** using laws of planetary motion
- **Uncertainty propagation** for rigorous error estimation

All computations were done in Python using tools like `numpy`, `scipy`, `photutils`, `rawpy`, and `matplotlib`.

---

## 🧠 Key Data Science Skills Demonstrated

- **Data acquisition under constraints**: custom imaging in remote, low-light conditions
- **Image preprocessing**: RAW file parsing, Gaussian filtering, pixel-level masking
- **Custom object detection**: `DAOStarFinder` + centroid-based Jupiter localization
- **Coordinate transformation**: pixel → physical distance (km) using telescope specs
- **Curve fitting**: sinusoidal orbit modeling using non-linear least squares
- **Physical modeling**: application of Kepler’s law to infer planetary mass
- **Error analysis**: Gaussian uncertainty propagation on multivariate functions
- **Visualization**: orbit plots, fit comparisons, residual inspection

---

## 📁 Repository Structure

```bash
.
├── 01_data_preprocessing.ipynb     # Image loading, moon detection, Jupiter localization
├── 02_orbit_fitting_mass_estimation.ipynb  # Curve fitting, mass computation, error analysis
├── Report.pdf                      # Full scientific report with equations, plots, and discussion
└── README.md                       # Project overview and technical summary

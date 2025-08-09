Supplementary Dataset and Materials — A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset

This repository contains all supplementary materials, datasets, and figures used in the manuscript:

LeFevre, S. W. (2025). A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset. Submitted to Space Weather (AGU).

It includes the full event dataset with embedded formulas, model calculations, figure source files, and supplemental tables referenced in the manuscript. All data are provided in accessible formats to support transparency, reproducibility, and peer review.

Repository Contents
1. Data Files
LeFevre Substorm Model - Full Dataset with calculations.xlsx
Full dataset of 60 auroral substorm events from 2001–2025.
Contains observed charging times, calculated coupling parameters (Lf), scaling constants (Cs), and response factors (Rf).
All formulas are embedded in the Excel file for verification and reproduction of results.
Includes conditional formatting and sorting for easier filtering of regimes.

Table_1.xlsx
Data subset for Table 1 in the manuscript (20 representative events).
Contains XDst, start method, charging time, and model errors for both Lf-Rf and N-Rf methods.

Table_2.xlsx
Statistical summary for Table 2 in the manuscript, grouped by XDst bins.

Table_S1.xlsx (Supplemental)
Complete dataset of all events with additional metadata, timing method notes, and calculated parameters.

Table_S2.xlsx (Supplemental)
Additional statistical analysis outputs not included in the main manuscript.

2. Figures
All figures used in the manuscript are provided as high-resolution JPEGs for publication.

Figure1.jpg — GOES trace example for substorm onset and charging phase identification.

Figure_2.jpg — Clock angle weighting comparison between models.

Figure_3.jpg — Response factor trends (Lf-Rf vs. N-Rf).

Figure_4.jpg — Static Cs vs. dynamic Rf error comparison.

Figure_5.jpg — Two-regime behavior of Tdelay vs. XDst.

Figure_6.jpg — Prediction error vs. coupling strength and IMF clock angle.

3. Manuscript
A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset.docx

Full working draft of the manuscript prepared for submission to Space Weather.

Includes all figure references, table captions, and equations.

Supplemental tables are referenced and will be linked to this repository upon acceptance.

🛰 Model Overview
This study presents a dual-component empirical model for predicting auroral substorm onset timing in real time:

Loading Function (Lf) — Modified from Newell et al. (2007) with a reduced clock angle exponent (sin^(1/3)(θ/2)) to better capture onset delays under moderate IMF orientations.

Response Function (Rf) — Dynamic scaling factor derived from event-specific Cs constants as a function of coupling strength (XDst = V·|Bz| / 100). Exhibits a two-regime structure with a threshold at XDst ≈ –75.

The model achieves:

Mean absolute error: ~18 minutes

Standard deviation: ~13 minutes

N = 60 substorm events (2001–2025)

Robust performance under weak and transitional coupling conditions, where traditional models tend to fail.

📄 How to Cite
If you use this dataset, figures, or code in your work, please cite:

LeFevre, S. W. (2025). Supplement to: A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset. Zenodo. https://doi.org/10.5281/zenodo.16784026

BibTeX:

@dataset{lefevre2025_substorm_supplement,
  author = {LeFevre, Scott W.},
  title = {Supplement to: A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset},
  year = {2025},
  publisher = {Zenodo},
  doi = {10.5281/zenodo.16784026},
  url = {https://doi.org/10.5281/zenodo.16784026}
}
🔍 Reproducibility Notes
All formulas for Lf, Cs, Rf, and timing error are embedded in LeFevre Substorm Model - Full Dataset with calculations.xlsx and can be reviewed or modified directly.

Event timing determinations are based on GOES magnetometer Hp traces following the methodology in Section 2.2 of the manuscript.

XDst threshold of –75 separates weak and strong coupling regimes for Rf fitting.

📬 Contact
For questions about the dataset or model, contact:
Scott W. LeFevre
Email: (add your preferred email or ORCID here)
GitHub: SWL713

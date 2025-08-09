LeFevre (2025) – Supplemental Data and Materials
A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset
Supplemental repository for the manuscript submitted to Space Weather (AGU)
DOI: 10.5281/zenodo.16784026

Overview
This repository contains all supplemental datasets, figures, and tables used in the study:

LeFevre, S.W. (2025), A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset, Space Weather, [submitted].

The study presents a new empirical model for forecasting auroral substorm onset timing in real time using upstream solar wind measurements and GOES magnetometer data.
Unlike traditional coupling models optimized for geomagnetic activity intensity, this model predicts timing by combining:

A modified loading function (Lf) with reduced IMF clock angle weighting

A dual-regime dynamic response factor (Rf) tied to coupling strength proxy XDst

Definition of XDst
XDst is defined as:
XDst = V · |Bz| / 100,   for Bz < 0
where:
V = solar wind speed in km/s
Bz = GSM z-component of IMF in nT (southward negative)
Positive Bz values are excluded

XDst serves as a Dst-proxy coupling strength index, identifying the transition between weak/stable tail loading and strong/dynamic onset regimes.

Contents
Data Tables
Table_1.xlsx – Example subset of 20 auroral substorm events showing observed parameters, calculated Rf values for both Newell-based and Lf-based models, and absolute prediction errors.

Table_2.xlsx – Summary prediction error statistics for all 60 events, binned by coupling strength regime.

Table_S1.xlsx – Full dataset of 60 substorm events used in the study. Includes event metadata, start type, observed charging time, all solar wind parameters, and calculated Lf, Cs, and Rf values.
Note: All calculation formulas are embedded in this Excel file for transparency and reproducibility.

Table_S2.xlsx – Expanded results table with intermediate values used for figures and regression analysis.

Figures
(High-resolution JPG versions of manuscript figures)

Figure1.jpg – Example GOES magnetometer trace showing loading and onset identification.

Figure_2.jpg – Comparison of clock angle weighting functions.

Figure_3.jpg – Rf vs XDst response fits for Lf-based and Newell-based coupling.

Figure_4.jpg – Prediction error comparison: static Cs mean vs dynamic Rf.

Figure_5.jpg – Two-regime delay behavior vs XDst.

Figure_6.jpg – Prediction error vs XDst and IMF clock angle.

Primary Dataset
LeFevre Substorm Model - Full Dataset with calculations.xlsx – Master dataset with all events, calculations, and intermediate results.
Formulas for Lf, Rf, and all intermediate terms are embedded for verification.

Data Sources
All source data are from publicly available repositories:

OMNIWeb: https://omniweb.gsfc.nasa.gov/

NOAA SWPC: https://services.swpc.noaa.gov

NASA CDAWeb: https://cdaweb.gsfc.nasa.gov/

LASP Space Weather Data Portal: https://lasp.colorado.edu/space-weather-portal/

How to Cite
If you use this dataset or code in your own work, please cite:

LeFevre, S.W. (2025), A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset, Space Weather, [submitted].

License
Unless otherwise noted, all files are released under the Creative Commons Attribution 4.0 International License (CC BY 4.0).
You are free to share and adapt with appropriate credit.

Contact
Author: Scott W. LeFevre
Email: [scott.w.lefevre@gmail.com]
For questions about the data, methods, or replication, please open an Issue in this repository or email directly.

Notes for Reviewers
This repository contains all supplemental data referenced in the manuscript, with filenames matching table/figure labels in the paper.

All Excel datasets contain fully embedded calculation formulas for transparency.

Figures are provided as high-resolution images suitable for verification against manuscript visuals.

No proprietary or restricted-access data were used; all sources are open and listed above.

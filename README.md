A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset
Overview
This repository contains the full supplemental dataset, figures, and calculation resources for the study:

LeFevre, S.W. (2025), "A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset," submitted to Space Weather (AGU).

The model predicts the delay between solar wind–magnetosphere coupling onset and auroral substorm onset using:

A modified solar wind coupling function (Loading Function, Lf) optimized for shallow IMF clock angles.

A dynamic, regime-dependent response factor (Rf) scaled by a coupling strength proxy (XDst).

A two-regime behavior reflecting distinct magnetotail responses under weak and strong coupling.

The framework is designed for real-time auroral nowcasting, with particular value for mid-latitude aurora forecasting, and is based on 60 auroral substorm events (32 visually confirmed at mid-latitudes).

Repository Structure
Main Manuscript
A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset.docx
Full submission manuscript with methods, results, discussion, and references. Figures and tables are referenced in text.

Figures
Figure_1.jpg – Example GOES magnetometer trace with growth phase (G) and expansion phase (E) markers.

Figure_2.jpg – IMF clock angle coupling threshold analysis and comparison of angular weighting functions.

Figure_3.jpg – Response factor (Cs) trends for present vs. Newell-based coupling.

Figure_4.jpg – Prediction error comparison: static mean Cs vs. dynamic Rf model.

Figure_5.jpg – Two-regime behavior of substorm delay time (Tdelay) vs. XDst.

Figure_6.jpg – Prediction error vs. XDst and IMF clock angle for present vs. Newell-based model.

Primary Data Tables
Table_1.xlsx – Example subset of 20 events with key parameters and timing errors for both models.

Table_2.xlsx – Summary statistics for the full 60-event dataset, grouped by coupling regime.

Supplemental Tables
Table_S1.xlsx – Full 60-event dataset with solar wind parameters, coupling function values, and timing results.

Table_S2.xlsx – Supporting calculations, including intermediate parameters for reproducibility.

Note: All formulas used for Lf, Rf, XDst, and Tdelay calculations are embedded in the Excel sheets, enabling full reproduction and verification of results.

Data Sources
All solar wind and geomagnetic data used are publicly available:

Solar Wind:

OMNIWeb (pre-June 2025): https://omniweb.gsfc.nasa.gov/

NOAA SWPC real-time data (post-June 2025): https://services.swpc.noaa.gov

NASA CDAWeb L1 data (WIND, DSCOVR): https://cdaweb.gsfc.nasa.gov/

GOES Magnetometer:

LASP Space Weather Data Portal: https://lasp.colorado.edu/space-weather-portal/

NASA CDAWeb archive

Model Summary
1. Coupling Strength Proxy (XDst)
XDst = (V × |Bz|) / 100, with Bz < 0 only

Scales like the Dst index.

Serves as the predictor for Rf regime separation at XDst ≈ –75.

2. Loading Function (Lf)
Modified from Newell et al. (2007):
Lf = V^(4/3) × Bt^(2/3) × sin^(1/3)(θ/2)

Uses fractional sine exponent (1/3) to better capture timing under moderate clock angles (~30°–50° threshold).

3. Response Function (Rf)
Empirically fit to observed scaling constants (Cs) vs. XDst:

Weak Coupling (XDst > –75): 2nd-order polynomial

Strong Coupling (XDst ≤ –75): 3rd-order polynomial

Captures:

Weak regime: Longer, more variable delays due to plasma sheet stabilization.

Strong regime: Shorter delays with rebound under extreme driving (possible feedback/saturation effects).

4. Timing Prediction
Tdelay = Rf / Lf

Applied from growth phase onset to predict expansion onset timing.

Key Findings
Mean timing error: 18 minutes (σ = 13 min) across all 60 events.

Performance gain over Newell-based coupling:

Especially in weak and transitional regimes, avoiding multi-day overpredictions.

Stable across full XDst range and IMF clock angles.

Physically grounded two-regime behavior: Matches trends reported by Freeman & Morley (2004) and Hsu & McPherron (2002).

Reproducibility
All calculation formulas are embedded in the Excel sheets (Table_1.xlsx, Table_S1.xlsx).

No proprietary code—Microsoft Excel and JMP 17.0.0 used for analysis.

Datasets span 2001–2025, covering multiple solar cycles and a wide intensity range.

How to Use
Download this repository.

Open LeFevre Substorm Model - Full Dataset with calculations.xlsx to view the full dataset with embedded formulas.

Adjust input solar wind parameters in the provided template to test your own event predictions.

Use Figures 2–6 for reference on model behavior under different coupling strengths and IMF conditions.

Citation
If using this dataset or model in your own work, please cite:

LeFevre, S.W. (2025), A Real-Time Loading–Response Model for Predicting Auroral Substorm Onset, Space Weather (submitted).

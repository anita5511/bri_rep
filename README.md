README.md File Documentation

# EEG Signal Processing and Classification

This repository contains the complete codebase, execution notebooks, and comprehensive analysis for 8 structural research assignments completed during my 3-month engineering internship at Brainwave Science.

##  Repository Layout
├── Assignment_1_CSP_LDA_MotorImagery.ipynb
├── Assignment_2_Subject_Wise_Performance.ipynb
├── Assignment_3_Band_Wise_Analysis.ipynb
├── Assignment_4_CSP_Variants_Review
├── Assignment_5_DREAMER_Riemannian.ipynb
├── Assignment_6_DREAMER_Method_Comparison.ipynb
├── Assignment_7_DREAMER_LOSSO_Validation.ipynb
└── Assignment_8_Findings_Conclusions

## Assignment Summaries & Quick Run Guide

### [Assignment 1] EEG Motor Imagery Classification (CSP + LDA)
- Implements a baseline BCI engine utilizing 5th-order Butterworth filtering (8-30 Hz) coupled with Common Spatial Patterns and Linear Discriminant Analysis on the PhysioNet EEGMMIDB dataset.
- Key Modules: `mne.decoding.CSP`, `sklearn.discriminant_analysis.LinearDiscriminantAnalysis`.

### [Assignment 2] Subject-wise Performance Profile
- Population study across all 109 subjects of the PhysioNet data to graph distribution variance, identify top performing outliers, and evaluate BCI Illiteracy.

### [Assignment 3] Band-wise EEG Signal Analysis
- Breaks down the input space into isolated bands (Delta, Theta, Alpha, Beta, Gamma) to rank spectral bands based on performance metrics.

### [Assignment 4] Comparative Study of CSP Variants
- A mathematical and theoretical architectural matrix evaluating 10 distinct variants of the CSP algorithm.

### [Assignment 5] DREAMER Emotion Classification
- Implements an information-geometric approach on the DREAMER dataset for Valence classification using a Riemannian Minimum Distance to Mean (MDM) classifier.
- Key Modules: `pyriemann.classification.MDM`, `pyriemann.estimation.Covariances`.

### [Assignment 6] DREAMER Method Comparison
- A benchmarking module comparing classical workflows against non-linear variations (CSP+LDA vs CSP+SVM vs FBCSP+LDA vs FBCSP+SVM).

### [Assignment 7] DREAMER LOSSO Validation
- Tests structural generalized deployment via Leave-One-Subject-Out protocols across 23 subjects.

### [Assignment 8] Research Findings & Future Outlook
- Consolidates all empirical data, insights, and structural recommendations for future production implementations.

##  Setup & Execution

Ensure your Python environment satisfies the dependencies listed below:
```bash
pip install numpy pandas scipy matplotlib seaborn scikit-learn mne pyriemann
```
Open any desired Jupyter Notebook sequentially to run the full processing loop:
```bash
jupyter notebook EEG_Motor_Imagery_Classification.ipynb
```


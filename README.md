# Prediction of the Intensity of Physical Movement of Aged People

This repository contains the experimental notebooks for the study: "Prediction of the Intensity of Physical Movement of Aged People". The project explores machine-learning approaches for estimating movement intensity in older adults using low-cost gas sensor data, with emphasis on noise reduction and feature engineering.

## Overview

Real-time monitoring of elderly people can improve health management, but camera-based systems raise privacy and cost concerns. This work evaluates sensor-based alternatives using gas-sensor readings to infer movement intensity. The study compares several preprocessing strategies and machine-learning models to predict activity intensity from noisy sensor data.

## Key contributions

- Sensor data preprocessing with:
  - raw signal
  - rolling-average smoothing
  - Gaussian-based noise reduction
  - true-value estimation
- Feature generation from statistical and time-domain sensor characteristics
- Feature selection to retain the most informative features
- Evaluation of multiple classifiers:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - XGBoost
  - Gaussian Naive Bayes
  - Ensemble methods

## Reported results

The study reports that the best-performing approach achieved approximately 78% accuracy using the true-value prediction preprocessing pipeline with an ensemble model. The lowest accuracy was observed for the raw-data logistic regression baseline.

## Repository structure

This repo is primarily a notebook-based experiment archive. Main files include:

- `A_data_cleaning_and_processing_v1.ipynb`
- `B_feature_generation_and_selection_v1.ipynb`
- `C_movement_prediction_v1.ipynb`
- `Model_*.ipynb` files for individual model experiments
- `gaussian_filter*.ipynb` for noise-reduction experiments
- `anomaly detection_v1.ipynb` for exploratory analysis

## Getting started

1. Install dependencies:
   ```bash
   pip install jupyter pandas numpy scikit-learn xgboost matplotlib seaborn
   ```
2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Open the notebooks in order, starting with the preprocessing and feature-generation notebooks.

Note: If the original dataset is not included in this repository, you may need to add it locally before running the notebooks.

## Publication

IEEE paper: https://ieeexplore.ieee.org/document/10534390

## Citation

If you use this work, please cite the paper linked above.

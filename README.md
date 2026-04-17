# Advanced ADHD Classification from Resting-State Functional Connectivity

## Overview

This repository was developed as a direct methodological follow-up to a baseline ADHD classification study (Repo 3), which applied a simple logistic regression model to resting-state fMRI functional connectivity features and obtained limited predictive performance.

Rather than treating those results as failure, this project uses them as motivation for a more rigorous second-stage analysis incorporating expanded data usage, feature selection, and model comparison.

The repository therefore demonstrates an iterative scientific workflow: identify limitations, redesign methodology, and reassess performance.

---

## From Repo 3 to Repo 4

## Baseline Study (Repo 3)

**Approach**

* Logistic Regression only
* Smaller subset analysis
* Basic feature pipeline
* Single-model evaluation

**Findings**

* Accuracy: 0.20
* ROC-AUC: 0.04

**Key Limitations Identified**

* Very small sample
* High-dimensional feature space
* No model benchmarking
* No feature selection
* Limited robustness

---

## Current Study (Repo 4)

## Improvements Introduced

* Expanded cohort usage
* Cohort audit (class balance, age, site distributions)
* SelectKBest feature selection
* Multi-model benchmarking
* Stratified cross-validation
* Feature importance analysis
* Improved result interpretation

---

## Research Question

Can methodological improvements enhance ADHD vs control classification from resting-state functional connectivity?

---

## Methods

### Data

* Public ADHD resting-state fMRI cohort
* Multi-site participants
* ADHD and control labels

### Neuroimaging Pipeline

* Harvard-Oxford atlas ROI extraction
* ROI time-series preprocessing
* Functional connectivity matrices
* Upper-triangle feature vectors

### Models Compared

* Logistic Regression
* Linear SVM
* Random Forest

### Evaluation

* Accuracy
* ROC-AUC
* F1-score
* Confusion Matrix
* ROC Curve

---

## Results

| Model               | Accuracy | ROC-AUC |       F1 |
| ------------------- | -------: | ------: | -------: |
| Logistic Regression |     0.37 |    0.28 |     0.21 |
| Linear SVM          |     0.43 |    0.34 |     0.18 |
| Random Forest       | **0.47** |    0.33 | **0.33** |

### Best Model

Random Forest achieved the strongest overall balance of metrics.

---

## Figures

### Model Performance Comparison

![Model Performance Comparison](./figures/model performance.png)

### Random Forest Confusion Matrix

![Random Forest Confusion Matrix](./figures/Random forest confusion.png)

### Random Forest ROC Curve

![Random Forest ROC Curve](./figures/Random Forest ROC.png)

### Top Connectivity Features

![Top Connectivity Features](./figures/Top connectivity features.png)

---

## Interpretation

Performance remained modest, but the project successfully improved upon the baseline pipeline and demonstrates that methodological choices materially influence outcomes in clinical neuroimaging machine learning.

The continued difficulty of classification likely reflects broader challenges in ADHD biomarker research, including:

* Diagnostic heterogeneity
* Site effects
* Age-related variability
* Small sample size
* Limited signal-to-noise ratio

---

## Why This Repository Matters

This project is valuable not because it claims clinical prediction success, but because it demonstrates how researchers respond to weak initial findings through structured methodological refinement.

That process, rather than isolated scores, is central to real scientific progress.

---

## Future Directions

* Larger harmonised datasets
* Confound regression (age, motion, site)
* Nested cross-validation
* Explainable AI methods
* Graph-theoretic network features
* Multimodal prediction pipelines

---

## Skills Demonstrated

* Computational neuroimaging
* Functional connectivity analysis
* Machine learning benchmarking
* Feature selection
* Cross-validation
* Transparent scientific reporting
* Iterative research design

---

## Author

Aditya Sundaray

Computational neuroscience portfolio project for PhD/research applications.

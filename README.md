# COPOD Reproduction — Assignment 2

This repository contains my reproduction of the **COPOD (Copula-Based Outlier Detection)** algorithm for Assignment 2 of the Applied Data Science Master's programme at Utrecht University.

## Experiment

The reproduction was performed on the **BreastW** dataset used in the COPOD paper.

### Experimental settings

- **Dataset:** BreastW
- **Observations:** 683
- **Features:** 9
- **Training split:** 60%
- **Test split:** 40%
- **Number of runs:** 10
- **Random states:** 0–9
- **Standardization:** StandardScaler
- **Algorithm:** COPOD
- **Contamination:** 0.3499
- **Evaluation metrics:** ROC-AUC and Average Precision

## Results

| Metric | Paper | Reproduction | Standard Deviation |
|---|---:|---:|---:|
| ROC-AUC | 0.9936 | 0.9935 | 0.0029 |
| Average Precision | Not reported | 0.9877 | 0.0052 |

The reproduced ROC-AUC differs from the value reported in the paper by only **0.000102 (−0.0102%)**.

## Contents

- `Assignment_2_COPOD_Reproduction.ipynb` — notebook containing the complete reproduction experiment.

## Reference

Rekatsinas et al., *COPOD: Copula-Based Outlier Detection*, ICDM 2020.

The original COPOD implementation and supplementary material are available in the authors' repository:

https://github.com/winstonll/COPOD

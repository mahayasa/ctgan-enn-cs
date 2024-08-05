# Optimizing CTGAN-ENN in Customer Churn Prediction: A Cost-Sensitive Learning Perspective
[![PyPI version](https://badge.fury.io/py/ctganenn.svg)](https://badge.fury.io/py/ctganenn)
[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)](https://badge.fury.io/py/ctganenn)

## Introduction
we aim to enhance the performance of several classical machine learning algorithms, including Decision
Trees (DT), Logistic Regression (LR), and Support Vector Machines (SVM), in customer churn
prediction tasks using CTGAN-ENN and cost-sensitive learning method.

## Objectives
- Optimizing customer churn prediction result by extend the CTGAN-ENN with cost-sensitive learning perspective
- Evaluate the performance of prediction using F1-score, AUC, and G-Mean metric
- Ivestigate how robust is the classical machine learning algorithm on this area

## Methodology
<img src="https://github.com/mahayasa/ctgan-enn-cs/blob/main/image/ctgan-enn.jpg" alt="Sample Image" width="70%">
CTGAN was used to generates synthetic data to augment the minority class, resulting in a set of generated data.
The new dataset is further processed with ENN which aims to remove noisy or ambiguous instances by identifying and eliminating overlapping data points.
The details of framework result can be accessed <a href="https://github.com/mahayasa/gan-hybrid-sampling-customer-churn">here</a>

<br><br>

<img src="https://github.com/mahayasa/ctgan-enn-cs/blob/main/image/ctgan-enn-cs.png" alt="Sample Image" width="70%">
The objective of CTGAN-ENN-CS is fine-tuning on hyperparameter of the lassifier in 𝑐𝑙𝑎𝑠𝑠_𝑤𝑒𝑖𝑔ℎ𝑡 hyperparameter. This involves adjusting the weights assigned to the classes in the loss function to handle class

## Results
CTGAN-ENN-CS framework surpasses the CTGAN-ENN on average on AUC-ROC, F1-Score, and G-Mean evaluation metrics, the result also shows CTGAN-ENN-CS was more robust than CTGAN-ENN in all classical machine learning algorithms.


### Key Findings
- CTGAN-ENN-CS improved (DT,SVM,LR) Classical machine learning performance on customer churn prediction on average
- CTGAN-ENN-CS was the most robust performance on (DT,SVM,LR)
- The most siginificant improvement by CTGAN-ENN-CS was SVM



## Future Work
Experiments another hybrid combination on CTGAN method such as adding anomaly detection method on CTGAN to make sure the synthetic data produced are not outliers.


---
<p align="left">
<img src="https://github.com/mahayasa/gan-hybrid-sampling-customer-churn/blob/main/image/kku.png" alt="Sample Image" width="20%">
<img src="https://github.com/mahayasa/gan-hybrid-sampling-customer-churn/blob/main/image/coc1.png" alt="Sample Image" width="20%">
</p>
This research was conducted as part of ASEAN GMS grant and part of AIDA
(Applied Intelligence and Data Analytics) lab in College of Computing, Khon Kaen University,
Thailand.


## Cite this work
<!--```bibtex
@misc{yourlabel,
  author = {Author(s) Name(s)},
  title = {Title of Research Project},
  year = {Year},
  howpublished = {\url{URL of the repository}}
}-->

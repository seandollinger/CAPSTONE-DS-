Predicting Circadian Rhythm Modulators: Feature Selection and Classification
Overview
This repository contains the code, datasets, and documentation for a project aimed at classifying molecules as changers or non-changers of circadian rhythms using chemical descriptors and machine learning. The project builds on work by Gul et al., leveraging a dataset of 88 molecules and integrating feature selection techniques to optimize classification performance. The study achieves significant improvements in predictive accuracy and provides insights into key molecular features driving circadian modulation.

Background
Circadian rhythms regulate essential biological processes through the interaction of core clock proteins like Cryptochromes (CRY). Dysregulation of these rhythms has been linked to various diseases, including cancer and mood disorders. This project explores the classification of small molecules that modulate circadian rhythms, contributing to drug discovery pipelines aimed at treating circadian-related disorders.

Key references:

Gul, S. et al., Structure-based design and classifications of small molecules regulating the circadian rhythm period.
Zhou, G. et al., An artificial intelligence accelerated virtual screening platform for drug discovery.
Objectives
Generate molecular descriptors for 88 molecules using the Paddle library.
Use feature selection techniques, including Random Forest and Recursive Feature Elimination (RFE), to optimize classification models.
Integrate descriptors from previous studies to improve classification accuracy and interpretability.
Develop a robust model capable of distinguishing changers and non-changers of circadian rhythms.
Project Workflow
Dataset Preparation

Molecules from Gul et al.'s dataset were analyzed to generate 215 chemical descriptors using the Paddle Python library.
Feature Selection

Random Forest was used to rank descriptor importance, reducing the dataset to 137 features (Set A).
Recursive Feature Elimination (RFE) was applied, resulting in a further refined set of 10 descriptors (Set B).
Model Development

Set B descriptors were combined with 10 descriptors identified by Gul et al. to create a final dataset (Set C).
Random Forest was used to evaluate performance, achieving a ROC AUC of 0.80.
Validation and Interpretation

10-fold cross-validation was performed to assess model variability.
Feature importance rankings were revisited to interpret molecular characteristics critical to classification.
Key Results
The integration of feature selection techniques and complementary datasets significantly improved classification accuracy and interpretability.
Final model (Set C) achieved:
Accuracy: 0.80
ROC AUC: 0.80

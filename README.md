
##  Project Overview
The objective of this project is to understand the importance of sampling techniques in handling imbalanced datasets.Credit card datasets are typically highly imbalanced, which can significantly skew model performance.This project involves balancing the dataset, applying five different sampling strategies, and evaluating their impact on five distinct machine learning models.

##  Methodology
1. **Data Acquisition**: Downloaded the credit card dataset provided in the assignment.
2. **Class Balancing**: Converted the imbalanced data into a balanced class dataset to ensure fair training.
3. **Sampling Implementation**: Created five samples using techniques taught in class: Simple Random, Systematic, Stratified, Cluster, and Bootstrap.
4. **Model Evaluation**: Applied five different ML models (M1-M5) to each sample and recorded the accuracy.



##  Results Matrix 
Based on the implementation, the following accuracy scores were obtained:

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **M1 (Logistic Regression)** | 93.51 | 89.61 | 89.61 | 85.53 | 93.51 |
| **M2 (Decision Tree)** | 98.70 | 97.40 | 92.21 | **100.00** | 98.70 |
| **M3 (Random Forest)** | **100.00** | **100.00** | 98.70 | 98.68 | **100.00** |
| **M4 (SVM)** | 67.53 | **75.32** | 64.94 | 71.05 | 72.73 |
| **M5 (KNN)** | 94.81 | 93.51 | 87.01 | **97.37** | 93.51 |

##  Discussion
* **Top Performer**: **Random Forest (M3)** demonstrated the highest consistency, achieving 100% accuracy in three out of five sampling scenarios.
* **Cluster Sampling Impact**: **Sampling 4 (Cluster Sampling)** yielded the best results for **Decision Tree** and **KNN** models, showing that grouping-based selection can capture representative patterns effectively for these algorithms.
* **Model Sensitivity**: **SVM (M4)** was the most sensitive to the sampling method, showing a significant performance boost with **Systematic Sampling** compared to others.
* **Conclusion**: Balancing the dataset is a critical first step; however, the choice of sampling technique significantly influences the final predictive accuracy depending on the model architecture used.


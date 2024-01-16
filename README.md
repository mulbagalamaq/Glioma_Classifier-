# Glioma-Classifier

# Title: Advanced Analytical Approach in Glioma Grading Using Clinical and Genetic Data ### 

- Author: Aymen Maqsood
- Date: 03/12/2023


## Introduction
This project represents a deep dive into the complexities of bioinformatics, with a specific focus on grading gliomas through the analysis of clinical and genetic data. My approach employs a range of statistical and machine learning techniques, underpinned by R's robust libraries. The goal is to develop reliable models that can accurately classify gliomas, enhancing our understanding and treatment of this condition.



## Description
Glioma is the most common cancer of the central nervous system and a leading cause of death due to poor prognosis. The treatment of gliomas greatly depends on accurate tumor classification. The mostly widely used WHO classification classifies gliomas into low grade (Astrocytoma, Oligodendroglioma) and high grade (Glioblastoma) based on their cells of origin. classifying gliomas to distinguish between the lethal high-grade glioblastoma and the low-grade gliomas is an unmet need and incorrect classification can greatly affect the treatment plan and its outcome.

This project used publicly available gene expression data and clinical information for glioma from The Cancer Genome Atlas (TCGA).

## Methodology
### Data Preparation and Exploration

#### Data Acquisition:
- The journey began with the data import using *TCGA_InfoWithGrade.csv*
- I placed a strong emphasis on treating categorical variables with care and ensuring data integrity.

#### Exploratory Data Analysis (EDA):
A comprehensive exploration of the data set was conducted, employing visualizations, and statistical tests like Chi-Square and ANOVA. This phase helped in understanding the data distribution, identifying patterns, and recognizing correlations.

### Model Development

#### Data Splitting Strategy: 

I split the dataset into a training set (75%) and a testing set (25%), adhering to best practices in data science for model validation.
Model Building: Four different machine learning models were constructed:

1. K-Nearest Neighbors (KNN): A model that classifies data points based on their proximity to neighbors.

2. Naive Bayes: A probabilistic model that applies Bayes' Theorem with strong independence assumptions between features.

3. Logistic Regression: A model used for binary classification tasks, predicting the probability of occurrence.

4. Support Vector Machine (SVM): A robust algorithm that finds a hyperplane in an N-dimensional space to classify data points.

Each model was chosen for its suitability in handling the mixture of categorical and continuous data typical in clinical datasets.

#### Model Evaluation
Metrics: To evaluate the models, I used a range of metrics including accuracy, precision, recall, F1 Score, and Area Under the ROC Curve (AUC). These metrics provided a comprehensive view of each model's performance and were particularly apt for the medical classification task at hand.

This project compares the performance of all four models for given data using a 10-fold Cross Validation

### Advanced Analytical Techniques

- Model Tuning
Fine-tuned each model to enhance their performance. For KNN, the number of neighbors was optimized, while for SVM, parameters like cost and gamma were adjusted.

- Ensemble Modeling
Developed an ensemble model that combined predictions from the individual models. This approach aimed to leverage the strengths of each model, potentially improving the overall predictive power.

## Conclusion
This project illustrates the power of machine learning in the field of medical diagnostics. The process of transforming raw clinical and genetic data into actionable insights through advanced analytics demonstrates the potential of data science in healthcare.



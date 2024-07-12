# ml-4-cyber-def

This repository contains a collection of Jupyter Notebooks that implement Machine Learning models for cyberattack classification, as well as metrics in CSV (Comma-separated values) format and a spreadsheet encompassing the results. The notebooks were created as part of an information security research project and were used to train and evaluate different machine learning algorithms, as well as preprocessing techniques and hyperparameter tuning to identify and classify types of cyberattacks.

## Notebooks

- [preprocessing.ipynb](scripts/preprocessing.ipynb): Notebook responsible for the preparation and preprocessing of the CSE-CIC-IDS2018 dataset used in model training.

- [preprocessing-kdd.ipynb](scripts/preprocessing-kdd.ipynb): Notebook responsible for the preparation and preprocessing of the KDD-1999 dataset used in model training.

- [ASSEMBLE_FINAL.ipynb](scripts/ASSEMBLE_FINAL.ipynb): Notebook that performs automated training of all Machine Learning models for cyberattack classification and generates metrics for analysis.

- [ASSEMBLE_FINAL_NO_PREPROC.ipynb](scripts/ASSEMBLE_FINAL_NO_PREPROC.ipynb): Notebook that performs automated training of all Machine Learning models for cyberattack classification and generates metrics for analysis with datasets that have not undergone preprocessing steps.

- Other Notebooks: The other notebooks test the performance of algorithms separately, implementing Random Forest, Decision Tree, Naive Bayes, Support Vector Machines, XGBoost, K-Neighbors, and Neural Network algorithms.

## Datasets

The datasets used for training and testing the models were [KDD-1999](https://kdd.org/kdd-cup/view/kdd-cup-1999) and [CSE-CIC-IDS2018](https://registry.opendata.aws/cse-cic-ids2018).

## Metrics

The following metrics are generated from the trained classification models:

- Accuracy: the proportion of correctly classified instances relative to the total number of instances.

- Precision: the proportion of correctly classified positive instances relative to the total number of instances classified as positive.

- Recall: the proportion of correctly classified positive instances relative to the total number of actual positive instances.

- F1-Score: the harmonic mean between precision and recall, providing a balanced measure between the two previous metrics.

- ROC-AUC: a performance measure used to evaluate the quality of a binary classification model. The ROC curve is obtained by plotting the true positive rate (TPR or recall) against the false positive rate (FPR or 1 - Specificity) for various classification threshold values.

The spreadsheet [Final Metrics.ods](metrics/Final%20Metrics.ods) centralizes all the .csv files, containing the results of the 3 analysis scenarios.
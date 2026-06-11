# MachineLearning-clinical-drug-classification-random-forest
An AI-driven clinical decision support system that automates drug categorization into five distinct classes using ensemble learning techniques.
# Multi-Class Drug Prescription Classification Using Random Forest
## Overview
In the domain of medical healthcare, accurate medication prescription is critical. This project implements a machine learning approach to automate the classification of therapeutic drugs based on patient physiological metrics. By utilizing a Random Forest classifier, this predictive model acts as an AI-driven decision support system to minimize human error and assist physicians in recommending appropriate treatments.  
## Dataset
The model is trained on the 'Drug Classification' dataset from Kaggle.  Size: 200 distinct patient records.  Features: 6 attributes, including Age, Sodium-to-Potassium Ratio (Na_to_K), Sex, Blood Pressure (BP), and Cholesterol.  Target Variable: Categorizes patients into one of five distinct drug classes: DrugY, drugA, drugB, drugC, and drugX.  
## Methodology
The data pipeline ensures robust model training through strict preprocessing standards:Preprocessing: Categorical variables were converted to numerical formats using Label Encoding, and extreme statistical outliers in the Na_to_K feature were removed using the Interquartile Range (IQR) method.  Data Partitioning: The data was stratified into an 80-20 split for training and testing.  Scaling: Standard Scalar Normalization was applied to ensure variables with larger magnitudes did not disproportionately influence the model.  Model: A Random Forest Classifier instantiated with 100 decision trees to mitigate variance.  
## Results
The ensemble method successfully distinguished between the five drug classes with minimal error.  Accuracy: Achieved an overall classification accuracy of 97.44%.  Efficiency: The model demonstrated rapid training times of under 1 second.  Generalization: Learning curve analysis confirmed low variance, indicating the model learned robust rules without overfitting.  
## Tech Stack
Language: Python
Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn 

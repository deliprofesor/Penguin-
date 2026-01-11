# 🐧 Penguin Species Classification and Biometric Analysis

<img width="1920" height="1080" alt="e-data kopyası" src="https://github.com/user-attachments/assets/5a0d7412-0b93-4c4c-99ec-4d215e9c4552" />


##  Project Summary
This project aims to develop a machine learning classification model that predicts the species of a penguin (Adelie, Chinstrap, or Gentoo) using its physical measurements (biometrics) and geographic location data collected around Palmer Station in Antarctica.

## Data Sources
The project utilizes two separate CSV files which are merged for a comprehensive analysis:

penguins_features.csv: Contains the penguin's species, sex, and four key biometric measurements (Culmen Length/Depth, Flipper Length, Body Mass).

penguins_location.csv: Contains the geographic region (Region) and the specific island (Island) where the penguin was observed.

Common Key: The two datasets are merged using the sample_id column.

## Methodology
The project follows four main stages, employing Exploratory Data Analysis (EDA) and Machine Learning (ML) techniques:

### Data Merging and Cleaning
Merging: The two datasets were joined using sample_id.

EDA (Missing Value Analysis): Initial missing (NaN) values were handled by dropping the corresponding rows to maintain the integrity of the biometric measurements.

Categorical Encoding: Categorical features such as Sex, Island, and Region were converted into a numerical format using One-Hot Encoding for model training.

### Model Development
Target and Features: The target variable (Y) is Species, and the features (X) include all biometric and encoded location characteristics.

Train/Test Split: The data was split into 80% training and 20% testing sets to assess the model's generalization ability.

Model Selection: The Random Forest Classifier was chosen for this multi-class classification task due to its robust performance and interpretability (Feature Importance).

### Results Evaluation (Evaluation and Feature Importance)
The model's performance on the test data was measured using Accuracy Score, and a Feature Importance analysis was conducted to understand which characteristics were most influential in predicting the species.

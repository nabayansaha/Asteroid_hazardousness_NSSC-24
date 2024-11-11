# Planetary Pookies NSSC'24 Data Analytics

## Team Information
Team: Planetary Pookies
Institution: IIT Kharagpur
Team Members:
- [Nabayan Saha](https://github.com/nabayansaha)
- [Shuvraneel Mitra](https://github.com/ShuvraneelMitra)
- [Srinjoy Das](https://github.com/SRINJOY59)
- [Agnij Biswas](https://github.com/Codeblade98)

## Project Overview

This project leverages data analytics and machine learning techniques to classify asteroids as hazardous or non-hazardous based on their physical and orbital characteristics. The primary objective is to identify asteroids that may pose a threat to Earth, enabling timely monitoring and potential mitigation.

## Objective of the Analysis
The main goal is to develop predictive models for classifying asteroids as hazardous or 
non-hazardous using features such as:
- Size
- Orbital parameters
- Velocity
- Proximity to Earth's orbit

Additionally, the project seeks to detect anomalous asteroids that may require further examination.

## Data Description
The dataset includes 24 features, out of which:
- 18 are numerical
- 6 are categorical

Some features are redundant, with physical quantities represented in different units.
Key attributes include: asteroid's name, relative velocity, miss distance, orbital period, and hazardous status.

## Methodology

### 1. Data Preprocessing
1. Imputation: Various methods were applied to handle missing values, such as forward and backward filling, linear interpolation, and iterative imputation for continuous data.
2. Feature Engineering: New features were generated, including the approach date, time until closest approach, and other orbital properties to enrich the dataset.
3. Normalization and Scaling: Distributions of numerical features were normalized to improve model performance.
4. Class Imbalance Handling: The dataset exhibited a class imbalance, which was addressed using SMOTE (Synthetic Minority Over-sampling Technique).

### 2. Statistical Analysis
- Descriptive Statistics: Initial data exploration, including range, mean, median, and standard deviation calculations.
- Correlation Analysis: Feature relationships were examined to detect redundancy and multicollinearity.
- Visualizations: Pair plots and histograms were used for exploratory analysis, showing bivariate relationships and feature distributions.

### 3. Machine Learning Models

# Hazardous Classification
- Model Selection: XGBoost and Random Forest Classifier with Recursive Feature Elimination (RFE) were used for feature selection.
- Hyperparameter Tuning: Both Bayesian Optimization and GridSearch techniques were applied.
- Cross-Validation: K-fold cross-validation was used to ensure reliable model evaluation.

# Anomaly Detection
- Isolation Forest and AutoEncoder were used to detect anomalies, such as rare or unusual asteroid behaviors.

## Evaluation Metrics
- Accuracy: 0.91
- AUC (Area Under Curve): 0.83
- Recall (weighted avg): 0.81
- F1-score (weighted avg): 0.82

These metrics highlight the model’s robustness, especially considering the class imbalance.

## Key Findings
- Significant correlations were found among certain features, suggesting possible redundancies.
- Anomalies were detected successfully, and both classification and anomaly detection models performed well in identifying potential threats.

## Conclusion
This analysis demonstrates the feasibility of using machine learning to assess asteroid threats and highlights the importance of feature engineering and handling class imbalance. The model provides a foundation for further research and refinement in predictive asteroid classification.

## Future Work
- Additional features could be incorporated, such as asteroid composition data.
- Model refinements and ensemble techniques may improve classification accuracy.

# ---
# Note: 
This project is by the 1st runners up team planetary pookies which is a part of the NSSC'24 initiative at IIT Kharagpur and serves as a crucial step towards planetary defense and asteroid hazard monitoring.

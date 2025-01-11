# Credit Card Behavior Score: IIT Bombay Case Study

## Introduction
This project aims to develop a predictive model for calculating the "Behavior Score" of credit card customers for Bank A. The score predicts the probability of a customer defaulting on their credit card, enabling robust risk management for the bank's existing portfolio.

## Problem Statement
The task is to build a behavior score using historical development data, predicting the probability of credit card defaults. The model will also be used to predict default probabilities on validation data for operational implementation.

## Datasets
- **Development Data**: 96,806 credit card records with `bad_flag` indicating defaults.
- **Validation Data**: 41,792 credit card records without `bad_flag`, for probability prediction.
- **Features Include**:
  - On-us attributes (credit limit, etc.).
  - Transaction-level attributes (transaction counts, merchant data).
  - Bureau tradeline attributes (historical delinquencies, holdings).
  - Bureau enquiry attributes (e.g., past enquiries).

## Approach
1. **Data Preprocessing**:
   - Handled missing values and standardized features.
   - Addressed data imbalance using SMOTE.
2. **Exploratory Data Analysis (EDA)**:
   - Analyzed feature correlations and distributions.
   - Investigated default patterns across customer segments.
3. **Model Development**:
   - Used Random Forest, LightGBM, and Gradient Boosting.
   - Conducted hyperparameter tuning using GridSearchCV.
4. **Model Evaluation**:
   - Evaluated models on metrics like AUC-ROC, PR-AUC, F1-score, G-Mean, and Matthews Correlation Coefficient.
   - Validated on unseen data, ensuring predicted probabilities were between 0 and 1.

## Results
- Developed a high-performing predictive model for credit card default risk.
- Provided actionable insights into customer behavior and portfolio risk.

## Repository Contents
- **Code**: Python scripts for data preprocessing, modeling, and evaluation.
- **Insights**: Key findings from EDA and model interpretations.
- **Documentation**: Detailed steps, metrics, and observations.

## Usage
1. Clone the repository.
2. Install required libraries using `requirements.txt`.
3. Run the scripts to preprocess data, train the model, and make predictions.

## Evaluation Metrics
- Threshold-Independent: AUC-ROC, PR-AUC.
- Threshold-Dependent: F1-Score, Confusion Matrix.
- Business Metrics: Weighted Cost Analysis.
- Class Imbalance: G-Mean, Matthews Correlation Coefficient, Cohen's Kappa.

## Conclusion
This project delivers a robust behavior score model, enabling Bank A to manage credit risk effectively. The insights and predictions support strategic decision-making and portfolio optimization.

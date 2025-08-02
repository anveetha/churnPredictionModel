# Customer Churn Prediction

## Author
Anveetha Suresh

## Project Overview

This project leverages machine learning to predict customer churn risk using a public dataset of user activity and demographics. Churn prediction is essential for businesses to retain valued customers and to allocate retention resources effectively.

Dataset Source:  
Kaggle User Churn Dataset ([Kaggle link](https://www.kaggle.com/datasets/fridrichmrtn/user-churn-dataset))

## Table of Contents

- [Installation](#installation)
- [Dataset Description](#dataset-description)
- [Notebook Sections](#notebook-sections)
- [How to Run](#how-to-run)
- [Results Summary](#results-summary)
- [Acknowledgments](#acknowledgments)

## Installation

To use this notebook, you will need the following packages:
- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib (if visualizations are present)
- jupyter

You can install the requirements using:
```bash
pip install pandas numpy scikit-learn matplotlib jupyter
```

## Dataset Description

The dataset contains the following columns:

- **age**: Age of the customer
- **gender**: Customer’s gender (M/F)
- **region_category**: Region where the customer lives (e.g., City, Village, Town)
- **membership_category**: Loyalty program or membership status
- **joined_through_referral**: Whether the customer joined via referral (Yes/No)
- **preferred_offer_types**: Customer’s preferred type of offer
- **medium_of_operation**: Device/platform used (Smartphone, Desktop, Both)
- **internet_option**: Internet connection type
- **days_since_last_login**: Days since customer's last login
- **avg_time_spent**: Average session duration
- **avg_transaction_value**: Mean value of customer transactions
- **avg_frequency_login_days**: Frequentness of logins
- **points_in_wallet**: Loyalty points
- **used_special_discount**: If customer used special discounts
- **past_complaint**: If customer has lodged any complaints
- **complaint_status**: Status of any complaints
- **feedback**: Customer feedback/reason for dissatisfaction
- **churn_risk_score**: Target variable (Risk of churn, presumably on a scale)

## Notebook Sections

1. **Data Loading**  
   Imports the dataset and checks for missing values.
2. **Data Preprocessing**  
   - Handles categorical variables via encoding
   - Converts columns to appropriate data types
   - Feature engineering as needed
3. **Data Exploration**  
   - Summary statistics
   - Data sample previews
4. **Modeling**  
   - Decision Tree Classifier is used to predict churn risk
   - Feature selection and one-hot encoding
   - Model training and evaluation
5. **Results and Insights**  
   - Evaluation metrics and sample predictions
   - Feature importances (if included)
   
---

## How to Run

1. Clone this repository or download the notebook.
2. Download the dataset from Kaggle (see above).
3. Place the CSV file in the same directory as the notebook or update the data loading path accordingly.
4. Launch Jupyter Notebook:
    ```bash
    jupyter notebook churnRisk.ipynb
    ```
5. Step through the notebook cells sequentially.

## Results Summary

- Each feature’s contribution to the churn risk is analyzed via a DecisionTreeClassifier.
- The notebook demonstrates preprocessing steps for categorical and numerical features.
- Evaluation metrics and sample outputs are displayed within the notebook for interpretability.

## Acknowledgments

- Dataset provided by [fridrichmrtn on Kaggle](https://www.kaggle.com/datasets/fridrichmrtn/user-churn-dataset)
- Notebook authored by Anveetha Suresh

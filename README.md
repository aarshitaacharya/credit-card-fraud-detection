# Credit Card Fraud Detection

Credit Card Fraud Detection is a critical application of machine learning in the finance industry. This project aims to develop a robust model to detect fraudulent transactions using a dataset from Kaggle.

## Introduction

Credit card fraud is a significant issue affecting financial institutions and consumers worldwide. Detecting fraudulent transactions is challenging due to their infrequency compared to legitimate transactions. This project explores various machine learning techniques to develop a fraud detection model.

## Dataset

The dataset used for this project is the [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud). It contains transactions made by credit cards in September 2013 by European cardholders. The dataset is highly imbalanced, with fraudulent transactions representing a small minority.

### Features

- Features V1 to V28: Anonymized numerical features derived from PCA.
- Time: Number of seconds elapsed between this transaction and the first transaction in the dataset.
- Amount: Transaction amount.
- Class: Target variable where `1` indicates fraud and `0` indicates a legitimate transaction.

## Data Preparation

- The dataset does not contain any missing values and does not require imputation.
- Numerical features are standardized for model comparison after balancing the dataset.
- The dataset is imbalanced, with the majority class being legitimate transactions (`Class 0`). Synthetic Minority Oversampling Technique (SMOTE) is used to address this imbalance.

## Exploratory Data Analysis

Exploratory analysis includes visualizations and statistical summaries to understand the distribution of transactions, explore temporal patterns of fraud, and analyze transaction amounts associated with fraud.

## Modeling

Various machine learning models such as Logistic Regression, Random Forest, and KNN are trained on the balanced dataset to predict fraudulent transactions. Model performance metrics like precision, recall, and F1-score are evaluated to assess the model's effectiveness.

## Evaluation

The K-Nearest Neighbors Classifier tuned with Grid Search performed exceptionally well:
- Best parameter: Euclidean Distance (p=2).
- Test accuracy: Nearly 99.8%.
- F1-Score: Achieved a perfect score.
- Minimal overfitting observed.

## Next Steps

- **Model Optimization**: Further fine-tuning of algorithms to enhance performance metrics.
  
- **Real-time Implementation**: Integration of the model into a real-time transaction monitoring system.
  
- **Continuous Improvement**: Regular updates and monitoring to adapt to new fraud patterns and ensure ongoing effectiveness.

## Conclusion

Credit card fraud detection is a complex problem that requires careful consideration of data imbalance, feature engineering, and model selection. This project demonstrates an approach to building an effective fraud detection system using machine learning techniques.

## References

- Kaggle Credit Card Fraud Detection Dataset: [Link](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- SMOTE: Synthetic Minority Over-sampling Technique: [Link](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html)


# customer-churn-prediction

End-to-end customer churn prediction project using machine learning techniques.

## Problem Statement
Customer churn is a critical challenge for subscription-based businesses.  
This project aims to predict whether a customer will churn based on their behavior, usage patterns, and subscription details.

## Dataset
The dataset contains customer-level information such as:
- Demographics (Age, Gender)
- Usage behavior (Usage Frequency, Support Calls)
- Payment behavior (Payment Delay, Total Spend)
- Subscription details (Subscription Type, Contract Length)

Target variable:
- **Churn** (0 = Not Churned, 1 = Churned)

## Data Preprocessing
- Removed missing values
- Encoded categorical variables:
  - Gender → Binary encoding
  - Subscription Type & Contract Length → One-hot encoding
- Feature scaling using **StandardScaler**
- Train-test split with stratification

## Models Used
###  Logistic Regression
- Scaled features
- Class imbalance handled using `class_weight='balanced'`
- Evaluation metrics:
  - Accuracy
  - Precision, Recall, F1-score
  - Confusion Matrix

### Random Forest Classifier
- Used for comparison
- Demonstrated significantly higher performance on the dataset

## Results
| Model | Accuracy |
| Logistic Regression | ~89% |
| Random Forest | ~99% |

Logistic Regression provides strong interpretability, while Random Forest achieves superior predictive performance.

## Confusion Matrix (Logistic Regression)
The confusion matrix highlights the trade-off between false positives and false negatives, which is crucial for churn prediction tasks.

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

## Future Improvements
- Hyperparameter tuning
- Feature importance analysis
- Cross-validation
- Deployment using FastAPI or Streamlit

## Author
**Talam**  
Aspiring Machine Learning / Data Analyst


# **Loan Approval Prediction**

This project addresses the challenge of predicting loan approval statuses based on demographic, financial, and loan-specific features. 
The objective is to assist financial institutions in streamlining loan approval processes while minimizing risk.

## **Data Source**
- A synthetic dataset inspired by credit risk analysis, consisting of 45,000 records and 14 features, including demographic, financial, and loan-specific attributes.
- Dataset from Kaggle: [Loan Approval Classification Dataset](https://www.kaggle.com/datasets/taweilo/loan-approval-classification-data/data)

## **Technologies Used**
- **Python** (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- **Jupyter Notebook**

## **Key Insights**
- **Credit Scores Matter**: Low credit scores are strongly correlated with loan rejections.
- **Income vs. Loan Amount**: Higher loan-to-income ratios increase rejection rates.
- **Loan Intent Trends**: Education loans have the highest rejection rates, while medical loans are most likely to be approved.
- **Model Performance**: Random Forest emerged as the best-performing model with an accuracy of 92.69% and an ROC-AUC score of 0.9735.

## **Modeling Approach**
- **Data Preprocessing**: Applied one-hot encoding, normalization, and standardization to prepare features for modeling.
- **Algorithms**: 
  - Logistic Regression (Baseline)
  - Random Forest (Best Performer)
  - K-Nearest Neighbors (KNN)
  - Naive Bayes
- **Evaluation Metrics**: 
  - Accuracy, Precision, Recall, F1-Score, ROC-AUC

| **Model**           | **Accuracy** | **Precision** | **Recall** | **F1-Score** | **ROC-AUC** |
|---------------------|--------------|---------------|------------|--------------|-------------|
| Logistic Regression | 89.58%       | 77.773%       | 74.41%     | 76.02%       | 0.9532      |
| Random Forest       | **92.56%**   | **89.59%**    | 75.22%     | **81.77%**   | **0.9721**  |
| KNN                 | 86.63%       | 73.15%        | 62.88%     | 67.62%       | 0.9025      |
| Naive Bayes         | 74.80%       | 46.78%        | **97.68%** | 63.26%       | 0.939       |

## **How to Run the Analysis**
1. Download the dataset from Kaggle.
2. Install the required Python libraries.
3. Run the `Loan_approval_rejection.ipynb` notebook to replicate the analysis and predictions.

## **Future Enhancements**
- Experiment with advanced models like XGBoost and LightGBM.
- Add explainability techniques (e.g., SHAP) to better interpret model predictions.
- Deploy the model via a web app for real-time loan approval predictions.

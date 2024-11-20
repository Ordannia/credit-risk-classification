Overview
========================
This analysis evaluates the credit risk of loans by predicting how likely they are to be healthy or high-risk.

The dataset used in this analysis contains financial information about loans, including the target variable, loan_status. This variable indicates the loan's status as either Healthy (0) or High-Risk (1).

Using features provided in the dataset, I aimed to build a machine learning model capable of predicting loan status. This involved:
    1. Splitting the data into testing and training sets to ensure an unbiased evaluation.
    2. Training a logistic regression model to predict whether a loan is healthy or high-risk.
    3. Evaluating the model's performance using accuracy, precision, recall and the F1 score.

Logistic regression was selected as the algorithm for this analysis because of its effectiveness in binary classification.
----------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------
Results
=======
Accuracy: 99%
Precision:
    - Healthy loans(0): 100%
        - This means 100% of predicted healthy loans were healthy
    - High-risk loans(1): 84%
        - This means 84% of predicted high-risk loans were high-risk
Recall:
    - Healthy loans(0): 99%
        - This means 99% of the healthy loans were caught
    - High-risk loans(1): 94%
        - This means 94% of the high-risk loans were caught
----------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------
Summary
=======
The logistic regression model demonstrated excellent performance in predicting healthy and high-risk loans
    - The healthy loans were predicted with a near perfect score. Precision was a perfect 100% while Recall was 99%. This means every loan predicted as healthy was healthy and almost all healthy loans were successfully identified.
    - The high-risk loans were predicted fairly well. Precision achieved only 84% and recall had a 94%. This means the majority of high-risk loans identified were actually high-risk and most of the high-risk loans were successfully identified.

Recommendation:
    Based on these results, I would recommend this model for use in identifying credit risk. The high accuracy and balanced recall for both healthy and high-risk loans make it suited for minimizing financial risk. Further threshold tuning could be explored to optimize performance if false positives for high-risk loans are a concern.
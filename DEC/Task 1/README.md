# Term Deposit Subscription Prediction (Bank Marketing)

## Objective
The objective of this project is to predict whether a bank customer will subscribe
to a term deposit as a result of a marketing campaign. By applying classification
models and explainable AI techniques, the goal is to improve customer targeting
and enhance the effectiveness of marketing campaigns.

---

## Dataset
**Bank Marketing Dataset (Full Version)**

The dataset was obtained from the UCI Machine Learning Repository and contains
information related to direct marketing campaigns of a Portuguese banking institution.
It includes 41,188 customer records with both demographic and campaign-related features.

**Target Variable:**
- `y` (1 = subscribed, 0 = not subscribed)

**Features:**
- Categorical: job, marital, education, contact, month, poutcome
- Numerical: age, balance, duration, campaign, pdays, previous

---

## Approach
The following steps were followed in this project:

1. Loaded and explored the dataset to understand customer attributes and campaign data
2. Encoded categorical variables using One-Hot Encoding
3. Scaled numerical features using StandardScaler
4. Split the dataset into training (80%) and testing (20%) sets
5. Trained classification models including Logistic Regression and Random Forest
6. Evaluated model performance using Confusion Matrix, F1-Score, and ROC Curve
7. Applied LIME to explain individual model predictions for selected customers

---

## Results & Insights
Both classification models demonstrated reasonable predictive performance. The
Random Forest classifier outperformed Logistic Regression in terms of F1-Score.
Analysis revealed that campaign-related features played a significant role in
determining customer subscription behavior.

---

## Model Performance
- **Logistic Regression:** Lower F1-Score compared to Random Forest
- **Random Forest:** F1-Score = 0.77 (Best Performing Model)

Key features influencing subscription decisions included:
- Duration of the last marketing call
- Contact communication type
- Number of previous contacts
- Month of contact

---

## Conclusion
This project demonstrates the effectiveness of machine learning models in predicting
term deposit subscription outcomes. By combining strong predictive performance with
explainable AI techniques such as LIME, the model provides both accuracy and
transparency, making it suitable for real-world banking marketing and decision
support systems.

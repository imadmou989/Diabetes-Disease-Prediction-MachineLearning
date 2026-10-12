# Diabetes Risk Prediction

Classic ML classifier predicting diabetes risk from clinical data, with statistical testing to justify feature choices before modeling.

## Data

[100,000 Diabetes Clinical Dataset](https://www.kaggle.com/datasets) (Kaggle) — clinical and demographic features, binary diabetes outcome.

## Approach

- Statistical testing (Shapiro-Wilk, Mann-Whitney U, chi-squared) to check feature-target relationships before feature selection.
- Preprocessing: label encoding for categoricals, standard scaling for numeric features.
- Models compared: Logistic Regression, Decision Tree, Random Forest.
- Evaluation: accuracy and classification report (precision/recall/F1) per class.

## Files

- `diabetes_risk_prediction.ipynb` — full pipeline: EDA, statistical tests, preprocessing, model training, evaluation.

## Run

Open in Jupyter or Google Colab. Requires `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `scikit-learn`.
# 🩺 Who's at Risk of Diabetes?

Exploratory analysis and a risk classifier on a clinical diabetes dataset (~100k patient records, 2015–2022, US states): who is most at risk, which factors matter, and how well simple models can flag high-risk patients.

`Python` · `pandas` · `seaborn` · `SciPy` · `scikit-learn`

## Analysis flow

1. **Inspect and clean** — types, missing values, class balancing
2. **Exploratory analysis** — distributions of age, BMI, HbA1c, blood glucose, smoking history, hypertension, and heart disease against diabetes status
3. **Drill-down** — risk by demographic group and comorbidity
4. **Statistical tests** — Shapiro–Wilk, Mann–Whitney U, and chi-square tests of association between risk factors and diabetes
5. **Prediction model** — logistic regression, decision tree, and random forest compared on the same split

## Files

- `Who's_at_Risk_of_Diabetes?_(with_Prediction_Model)_FINAL.ipynb` — final notebook ([open in Colab](https://colab.research.google.com/github/airimonda/diabetes_prediction_model/blob/main/Who's_at_Risk_of_Diabetes%3F_(with_Prediction_Model)_FINAL.ipynb))

## Limitations

- The positive class is rare, so accuracy alone overstates performance; precision and recall on the diabetic class are the metrics that matter.
- The data is observational; associations found here are not causal.

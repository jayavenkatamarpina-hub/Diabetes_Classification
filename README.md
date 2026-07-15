# Diabetes Prediction — Classification Model Comparison

Predicting diabetes using 5 classification models on a stratified 15,000-row sample of the diabetes prediction dataset (100,000 rows originally, ~91.5% no diabetes / 8.5% diabetes).

## What's in this notebook

- Encoded categorical features (gender, smoking_history)
- Took a stratified sample to keep training times reasonable, preserving the original class balance
- Trained and evaluated 5 models: Logistic Regression, KNN, Decision Tree, Naive Bayes, SVM
- Compared all 5 using accuracy, precision, recall, and F1-score
- Built a confusion matrix for the best performing model

## Result

Logistic Regression was selected as the best model, highest F1-score for the diabetes class (0.73) and tied for the best accuracy (0.96), while being simpler and faster than SVM. Decision Tree and Naive Bayes caught more true diabetes cases but with far more false positives, Naive Bayes especially, with precision dropping to 0.37.

## Files

- `Diabetes_Classification.ipynb` — the notebook
- `diabetes_prediction_dataset.csv` — the dataset

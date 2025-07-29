# IPL-score-prediction
Built a machine learning model to predict the final score of an IPL team based on match progression . Trained on historical IPL data (2008–2016) and tested on 2017 matches. Achieved the best performance using Linear Regression. Includes a prediction function for new match inputs and visual evaluations of model accuracy.

# 🏏 IPL Score Prediction using Machine Learning

This project predicts the final score of an IPL team during an ongoing match using match stats like overs, runs, wickets, and recent form.

---

## 📊 Project Overview

- Trained on IPL data from 2008–2016
- Tested on IPL 2017 data
- Uses Linear Regression, Random Forest, Decision Tree, AdaBoost
- Best model: **Linear Regression**

---

## 📂 Dataset

- Source: `ipl.csv`
- Columns used: `bat_team`, `bowl_team`, `overs`, `runs`, `wickets`, `runs_last_5`, `wickets_last_5`, `total`

---

## 🧠 Models Used

- Linear Regression ✅ *(Best)*
- Random Forest
- Decision Tree
- AdaBoost (with Linear Regression)

---

## 🧪 Features Used for Prediction

- Batting & Bowling teams (One-hot encoded)
- Overs
- Runs
- Wickets
- Runs and Wickets in last 5 overs

---

## 🚀 How to Use

1. Clone the repo  
2. Run the notebook `ipl_score_predictor.ipynb`  
3. Use the `predict_score()` function to predict outcomes  
4. You can also load the saved model with `joblib`

---

## 🔧 Tech Stack

- Python, Pandas, NumPy
- Scikit-learn, Matplotlib, Seaborn
- Jupyter Notebook

---

## 📈 Example Prediction

```python
sample_input = {
    'overs': 10,
    'runs': 82,
    'wickets': 2,
    'runs_last_5': 45,
    'wickets_last_5': 1,
    'bat_team_Mumbai Indians': 1,
    'bowl_team_Chennai Super Kings': 1
}

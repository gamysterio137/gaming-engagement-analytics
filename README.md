# 🎮 Gaming Engagement & Retention Analytics

This project analyzes online player behavior to predict user engagement levels (High / Medium / Low) and uncover insights to improve player retention and monetization strategies in mobile or online games.

---

## 📊 Dataset

- **Source**: [Kaggle – Predict Online Gaming Behavior Dataset](https://www.kaggle.com/datasets/rabieelkharoua/predict-online-gaming-behavior-dataset)
- **Features**: Demographics, play time, session metrics, in-game purchases, difficulty, achievements, game genre
- **Target**: `EngagementLevel` – classified into High, Medium, or Low

---

## 🔧 Tools & Libraries

- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (RandomForestClassifier, preprocessing, evaluation)

---

## 🧠 Problem Statement

Predict the level of engagement a player has with a game based on their behavior and profile data. Identify which player metrics are most influential and generate insights for retention-focused game design.

---

## 📈 Key Visuals

- Boxplots of session duration vs. engagement
- Violin plots of weekly session frequency
- Pairplots showing feature relationships by engagement level
- Feature importance chart (Random Forest)

---

## 📌 Key Insights Summary

- **Avg. Session Duration** and **Sessions Per Week** contribute over **60% of feature importance**, making them the strongest engagement indicators.
- **High Engagement** players log **15–20 sessions per week** and average **100–150 min/session**.
- **Low Engagement** players cluster around **0–5 sessions/week** with lower session durations.
- **PlayerLevel** and **AchievementsUnlocked** help but contribute less than core session metrics.
- **Demographics** (age, gender) are less predictive than in-game behavior.
- 📌 Recommendation: Introduce login-based streak rewards, optimize session flow, and surface personalized ads for Medium-engagement players.

---

## 🤖 Model

- Model: **Random Forest Classifier**
- Metrics: Precision, Recall, F1-Score (macro), Confusion Matrix
- Scaled features using `StandardScaler`

---

## 🗂 File Structure

```
📦 gaming-engagement-analytics
 ┣ 📘 Gaming_Engagement_Analysis.ipynb
 ┣ 📄 README.md
 ┗ 📊 dataset.csv (not included — download from Kaggle)
```

---

## 🚀 How to Run

1. Clone this repo or download the `.ipynb` file
2. Install requirements:
    ```bash
    pip install pandas seaborn scikit-learn matplotlib
    ```
3. Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
4. Run `Gaming_Engagement_Analysis.ipynb`

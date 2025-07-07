# SENTIMENT-ANALYSIS

NAME:BUSHRA AMATULLA

INTERN ID: CT04DG2674

DOMAIN:DATA ANALYSIS

DURATION: 4 WEEKS

MENTOR: NEELA SANTOSH

## 📁 Dataset Overview

- **Source**: Wine Reviews Dataset
- **Total Records**: ~130k (approx.)
- **Used Columns**:
  - `description`: Wine review text
  - `points`: Numerical rating of the wine (used to derive sentiment)
  
---

## 🧪 Sentiment Labeling

Sentiment was created based on the `points` column:
- ✅ **Positive (1)** → `points >= 90`
- ❌ **Negative (0)** → `points < 90`

---

## 🧹 Data Preprocessing Steps

- Removed missing values
- Cleaned text: lowercase, removed punctuation, numbers, and extra spaces
- Used **TF-IDF** Vectorization (`max_features=3000`)

---

## 🤖 Models Implemented

1. **Logistic Regression**
2. **Multinomial Naive Bayes**
3. **Support Vector Machine (SVM)**

All models were trained and evaluated using an 80/20 train-test split.

---

## 📊 Evaluation Metrics

- Accuracy Score
- Classification Report (Precision, Recall, F1-score)

---

## 📈 Results Summary

| Model               | Accuracy |
|--------------------|----------|
| Logistic Regression| ✅ ~85%   |
| Naive Bayes        | ✅ ~83%   |
| SVM (Linear)       | ✅ ~86%   |

> *(Note: Accuracy may vary depending on the dataset size and cleaning steps.)*

---

## 📝 Conclusion

- The SVM model gave the best performance.
- Clean review descriptions are good predictors of sentiment.
- This pipeline can be applied to other review datasets like tweets, product reviews, or comments.

---

## 💻 Tools & Libraries Used

- Python
- Pandas
- scikit-learn
- Regular Expressions (re)

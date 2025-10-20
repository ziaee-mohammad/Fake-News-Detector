# 📰 Fake News Detector

A **machine learning + NLP** project to detect fake news using **TF‑IDF** features and classical models (Logistic Regression, Naive Bayes, SVM, Random Forest).  
Includes a complete pipeline for text preprocessing, feature extraction, model training, and evaluation with standard classification metrics.

---

## 📖 Overview
This repository demonstrates an end‑to‑end workflow for **fake news detection** on labeled news headlines/articles.  
It covers:
- Text cleaning & normalization (lowercasing, punctuation removal, stopwords, lemmatization)
- Feature extraction with **TF‑IDF**
- Model training and hyperparameter tuning
- Evaluation via **Accuracy, Precision, Recall, F1**, and confusion matrix
- Reproducible notebooks and requirements

---

## 🗂️ Dataset
- Labeled news items containing text and target label (`fake` / `real` or `0/1`).  
- Typical columns: `id`, `title`, `text`, `label`.  
- Place your dataset under `Dataset/` (e.g., `Dataset/train.csv`, `Dataset/test.csv`).

> ⚠️ Make sure to verify class balance. If the dataset is imbalanced, consider class weights or resampling.

---

## 🧹 Preprocessing
- Tokenization, lowercasing, punctuation & number removal
- Stopword removal (NLTK)
- Lemmatization (WordNetLemmatizer) or stemming
- Optional: n‑grams (bi‑grams), max features cap, min_df thresholds

---

## 🧠 Models
- **Logistic Regression** (strong baseline for linear separable TF‑IDF spaces)
- **Multinomial Naive Bayes** (common baseline for sparse text features)
- **Linear SVM** (max‑margin, usually strong with TF‑IDF)
- **Random Forest** (non‑linear baseline; less common for sparse text but included)
- Optional: **XGBoost / LightGBM**

---

## 📈 Results (replace with your actual numbers)
| Model | Accuracy | Precision | Recall | F1 |
|------|---------:|----------:|------:|---:|
| Logistic Regression | 0.95 | 0.95 | 0.95 | 0.95 |
| Multinomial NB | 0.93 | 0.92 | 0.94 | 0.93 |
| Linear SVM | 0.96 | 0.96 | 0.96 | 0.96 |
| Random Forest | 0.90 | 0.90 | 0.90 | 0.90 |

> Include a confusion matrix and ROC/PR curves where appropriate.

---

## ⚙️ Project Structure
```
Fake-News-Detector/
├─ Dataset/                        # CSV files (train/test)
├─ Notebook/
│  └─ Fake_News_Detection.ipynb    # main analysis & modeling notebook
├─ src/                            # (optional) scripts if you modularize
│  ├─ data.py                      # loading / cleaning helpers
│  ├─ features.py                  # TF-IDF, vectorizers
│  ├─ train.py                     # training & evaluation
│  └─ utils.py
├─ reports/figures/                # plots (confusion matrix, PR/ROC)
├─ requirements.txt
├─ .gitignore
└─ README.md
```

---

## 🚀 Setup & Usage
1) **Clone & env**
```bash
git clone https://github.com/ziaee-mohammad/Fake-News-Detector.git
cd Fake-News-Detector
pip install -r requirements.txt
```

2) **Place data** under `Dataset/` (e.g., `train.csv`, `test.csv`).

3) **Run**  
- Open the notebook:
```bash
jupyter notebook Notebook/Fake_News_Detection.ipynb
```
- *(Optional)* If you add scripts:
```bash
python -m src.train --model "logreg" --ngrams 1,2 --max_features 100000
```

---

## 📦 Requirements (example)
```
pandas
numpy
scikit-learn
nltk
matplotlib
seaborn
xgboost           # optional
```
> Run `python -m nltk.downloader stopwords wordnet punkt` if needed.

---

## ✅ Reproducibility Tips
- Fix random seeds (`numpy`, `sklearn`)  
- Use stratified splits (`train_test_split(..., stratify=y)`)  
- Keep TF‑IDF + model in a single `Pipeline` to avoid leakage  
- Track and save vectorizers & models if you plan to deploy

---

## 🏷 Tags
```
data-science
machine-learning
nlp
text-mining
fake-news
classification
python
scikit-learn
tf-idf
logistic-regression
naive-bayes
svm
```

---

## 📜 License
MIT License — feel free to use and adapt with attribution.

---
## 👤 Author
**Mohammad Ziaee**  
📧 moha2012zia@gmail.com  
🔗 https://github.com/ziaee-mohammad
👉 Instagram: [@ziaee_mohammad](https://www.instagram.com/ziaee_mohammad/)

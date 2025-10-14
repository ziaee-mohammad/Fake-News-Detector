# 📦 Dataset — Fake News Detector

This folder contains the datasets used for training and evaluating the *Fake News Detection* models.

---

## 📄 Files
| File Name | Description |
|------------|-------------|
| train.csv | Labeled dataset used for model training |
| test.csv  | Evaluation dataset for testing model performance |

---

## 🧩 Structure
Each dataset contains the following columns:
| Column | Description |
|----------|-------------|
| id | Unique identifier for each article |
| title | Headline of the news article |
| text | Main text content of the news article |
| label | Binary target variable (1 = Fake, 0 = Real) |

---

## ⚙ Notes
- Missing values are handled during preprocessing.
- If you replace the dataset, ensure column names remain consistent.
- Class balance should be checked before training (imbalanced data may bias the model).

---

## 📚 Sources
You can use public datasets such as:
- [Kaggle: Fake News Detection](https://www.kaggle.com/c/fake-news)
- [Fake News Dataset by George McIntire](https://www.kaggle.com/datasets/george-mcintire/fake-news-data)

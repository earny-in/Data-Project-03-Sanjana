# Fake News Detection Dataset

## 📌 Overview

This dataset is used for the Fake News Detection project. The main goal of this project is to classify news articles as **Real** or **Fake**.

---

## 📂 Dataset Information

- **Dataset Name:** Fake News Dataset
- **File Format:** CSV
- **Rows:** 50
- **Columns:** 7

---

## 📊 Dataset Columns

| Column Name | Description |
|------------|-------------|
| title | Title of the news article |
| text | Complete news content |
| date | Publication date |
| source | Source of the news |
| author | Name of the author |
| category | Category of the news |
| label | Indicates whether the news is real or fake |

---

## 📁 Folder Structure

```text
Implementation/
│
├── data/
│   ├── fake_news_dataset.csv
│   └── README.md
```

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## 🎯 Project Objective

The objective of this project is:

- To analyze news articles.
- To preprocess the dataset.
- To train machine learning models.
- To classify news as real or fake.

---

## 🤖 Machine Learning Algorithms

The following algorithms can be used:

- Logistic Regression
- Naive Bayes
- Support Vector Machine (SVM)
- Passive Aggressive Classifier

---

## 💻 Load Dataset Using Python

```python
import pandas as pd

df = pd.read_csv("fake_news_dataset.csv")

print(df.head())
```

---

## 📌 Output Labels

- `real` → Real News
- `fake` → Fake News

---

## 📜 License

This dataset is intended for educational and research purposes only.
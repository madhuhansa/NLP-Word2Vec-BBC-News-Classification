# 🧠 BBC News Text Classification using spaCy Word Embeddings

This project performs **multi-class text classification** on the **BBC News Classification Dataset** using **spaCy’s pre-trained word embeddings**. It focuses on comparing classification models by transforming text into **dense semantic vectors** using `.vector` from spaCy, offering deeper meaning representation than TF-IDF or Bag-of-Words.

---

## 🔧 Technologies Used

- Python  
- spaCy  
- Scikit-learn  
- Pandas, NumPy  
- Jupyter Notebook  

---

## 📁 Dataset

The dataset contains **2,225 BBC News articles**, categorized into 5 classes:

- Business  
- Entertainment  
- Politics  
- Sport  
- Tech  

📌 Source: [Kaggle - BBC News Classification](https://www.kaggle.com/datasets/sunilthite/text-document-classification-dataset)

---

## 📌 Key Features

- Uses **spaCy pre-trained word embeddings** for feature extraction (`.vector`).
- Implements **average word vectors** to represent full articles.
- Applies **text preprocessing**: tokenization, lowercasing, stopword removal, etc.
- Trains and evaluates multiple ML models (Naive Bayes, Random Forest, etc.).

---

## ✅ Results & Observations

- Achieved **~95% accuracy** on test data.
- Word embeddings provide strong performance even without heavy feature engineering.
- Preprocessing enhances performance slightly by cleaning input to the vectorizer.

---

## 📁 Project Files & Folders Explained

| File/Folder | Description |
|-------------|-------------|
| `Model/` | Saved models using `joblib` for future prediction or reuse. |
| └── `logistic_regression_model.pkl` | logistic regression model trained on spaCy vectorized features. |
| `df_file.csv` | Cleaned dataset . |
| `model2.ipynb` | Main notebook: preprocessing, vectorization using spaCy, training, and evaluation. |
| `README.md` | This project overview and instructions. |

---

## 🤖 Difference from TF-IDF/BoW Projects

| Technique                  | Captures Context | Handles Synonyms | Requires Preprocessing | Used Here |
|---------------------------|------------------|------------------|------------------------|-----------|
| BoW                       | ❌                | ❌                | ✅                     | ❌        |
| TF-IDF                    | ❌                | ❌                | ✅                     | ❌        |
| Word Embeddings (spaCy)   | ✅                | ✅                | ✅ (optional)          | ✅        |

---

## 🙌 Credits

Project by **Yahan Madhuhansa**  
Inspired by advanced NLP applications using **spaCy**.

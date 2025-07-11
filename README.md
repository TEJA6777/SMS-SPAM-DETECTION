# 📩 Spam Detection Web App

This project is a **machine learning-based web application** that detects whether a given SMS or email message is spam or not. It uses various classification algorithms and provides a clean, user-friendly interface built with **Streamlit** for real-time message prediction.

---

## 🚀 Features

- Clean and interactive web interface built using Streamlit
- Accepts user input via text area to check for spam
- Preprocessing includes tokenization, stopword removal, and stemming
- Uses TF-IDF for vectorization
- Trained on a labeled SMS spam dataset
- Multiple algorithms evaluated for performance comparison

---

## 🤖 Algorithm Performance

The following machine learning models were trained and evaluated. Here are the results based on test set accuracy and precision:

| S.No | Algorithm                       | Accuracy  | Precision |
|------|----------------------------------|-----------|-----------|
| 1    | K-Nearest Neighbors (KN)         | 0.905     | 1.000     |
| 2    | Naive Bayes (NB)                 | 0.971     | 1.000     |
| 3    | Random Forest (RF)               | 0.976     | 0.983     |
| 4    | Support Vector Classifier (SVC)  | 0.976     | 0.975     |
| 5    | Extra Trees Classifier (ETC)     | 0.975     | 0.975     |
| 6    | Logistic Regression (LR)         | 0.958     | 0.970     |
| 7    | AdaBoost                         | 0.960     | 0.929     |
| 8    | XGBoost (XGB)                    | 0.967     | 0.926     |
| 9    | Gradient Boosting (GBDT)         | 0.947     | 0.919     |
| 10   | Bagging Classifier (BgC)         | 0.958     | 0.868     |
| 11   | Decision Tree (DT)               | 0.932     | 0.833     |

> ✅ **SVC** and **Random Forest** achieved the highest accuracy, while **Naive Bayes** scored perfect precision.

---

## 🧪 Dataset

- **Source**: [Kaggle - SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
- **Records**: 5,572 messages
- **Classes**: `ham` (not spam), `spam`

---

## 🖥 Streamlit Web App

### 🧩 Message Classification Flow:

1. User enters message text in the app.
2. Text is preprocessed:
   - Lowercasing
   - Tokenization
   - Removing stopwords and punctuation
   - Stemming
3. Transformed into TF-IDF vector
4. Model predicts whether it's spam or not

---

## 🗂️ File Structure


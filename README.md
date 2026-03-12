# Spam Mail Prediction using SVM

## Overview
This project builds a **Spam Mail Classifier** using **Support Vector Machines (SVM)**.  
The model processes SMS messages and predicts whether a message is **Spam** or **Ham (Not Spam)**.

The dataset contains labeled SMS messages where:
- `spam = 0`
- `ham = 1`

The model uses **TF-IDF vectorization** to convert text messages into numerical features and trains a **Linear SVM classifier** for prediction.

---

## Dataset
The dataset consists of two columns:

| Column | Description |
|------|-------------|
| v1 | Label (spam or ham) |
| v2 | SMS message text |

Example:

| v1 | v2 |
|----|----|
| ham | Ok lar... Joking wif u oni... |
| spam | Free entry in 2 a wkly comp to win FA Cup |

---

## Technologies Used

- Python
- NumPy
- Pandas
- Scikit-learn

Machine Learning Techniques:
- TF-IDF Vectorization
- Support Vector Machine (LinearSVC)

---

## Project Workflow

1. Load and preprocess dataset
2. Convert labels (`spam` → 0, `ham` → 1)
3. Split dataset into training and testing sets
4. Convert text messages into TF-IDF feature vectors
5. Train an **SVM classifier**
6. Evaluate model accuracy
7. Predict whether a new message is spam or ham

---

## Model Performance

| Metric | Score |
|------|------|
| Training Accuracy | **99.95%** |
| Test Accuracy | **98.56%** |

---

## Example Prediction

Input Message:
```
WINNER! As a valued network customer you have been selected to receive a $900 prize reward!
```

Output:
```
Spam Mail
```

---

## How to Run

1. Install required libraries

```bash
pip install numpy pandas scikit-learn
```

2. Run the Python script
```bash
python spam_classifier.py
```

---

## Future Improvements

- Use deep learning models (LSTM / BERT)
- Add preprocessing (stemming, lemmatization)
- Build a web API for predictions

---


# Data-Modeling---SVM-Logistic-Regression

# Spam Classification Using Logistic Regression and SVM

This project implements a spam detection model using **Logistic Regression** and **Support Vector Machines (SVM)**. The model classifies SMS messages as either **spam** or **ham** (not spam) using a dataset of labeled messages.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Technologies Used](#technologies-used)
4. [Project Structure](#project-structure)
5. [Model Evaluation](#model-evaluation)
6. [Results](#results)
7. [Future Improvements](#future-improvements)

---

## Project Overview

The purpose of this project is to build a classification model to detect spam messages using **machine learning** techniques. The dataset consists of SMS messages labeled as "ham" (non-spam) or "spam." The project covers:

- **Data preprocessing** (cleaning, encoding, vectorizing).
- **Exploratory Data Analysis (EDA)** to understand data distribution.
- Implementing **Logistic Regression** and **Support Vector Machines (SVM)**.
- Evaluating model performance using **accuracy**, **precision**, **recall**, and **confusion matrices**.

---

## Dataset

The dataset used is a collection of SMS messages with spam or ham labels. It contains the following columns:

- `v1`: Label ("ham" or "spam").
- `v2`: Message text.

### Example Data:
| Label | Message |
|-------|---------|
| ham   | "Hey, how are you doing?" |
| spam  | "Congratulations! You won a free ticket!" |

---

## Technologies Used

- **Python 3**
- **Pandas** for data manipulation
- **Seaborn** and **Matplotlib** for data visualization
- **Scikit-learn** for machine learning algorithms
  - Logistic Regression
  - Support Vector Machine (SVM)
  - CountVectorizer (Bag of Words)
  - Model evaluation metrics

---

## Project Structure

```
spam-classification/
│
├── data/
│   └── spam.csv              # Dataset file
│
├── images/                   # Visualizations and plots
│   ├── class_distribution.png
│   ├── message_length_distribution.png
│   ├── regression_message_length_spam.png
│   ├── logistic_regression_confusion_matrix.png
│   └── svm_decision_boundary.png
│
├── spam_classification.py    # Main script file
├── README.md                 # Project documentation
└── requirements.txt          # Dependencies
```

---

## Model Evaluation

Both models were evaluated using **accuracy**, **precision**, **recall**, and **confusion matrices**.

### Logistic Regression Performance:
- **Accuracy:** 97.87%
- **Precision:** 96.95%
- **Recall:** 87.59%

### Support Vector Machine (SVM) Performance:
- **Accuracy:** 98.16%
- **Precision:** 99.22%
- **Recall:** 87.59%

---

## Results

- **Support Vector Machine (SVM)** slightly outperformed **Logistic Regression** in terms of accuracy and precision.
- **Spam messages** tend to be longer, and this feature helped improve model performance.
- The models demonstrated strong potential for **real-world spam detection** in SMS applications.


---

## Future Improvements

1. **Hyperparameter tuning** using GridSearchCV.
2. Experimenting with **TF-IDF vectorization** for improved feature representation.
3. Testing additional models like **Naive Bayes** or **ensemble methods**.
4. Addressing **class imbalance** through techniques like oversampling.

---

**Author:** Sambad Rupakheti

Feel free to contribute or reach out if you have suggestions or improvements!

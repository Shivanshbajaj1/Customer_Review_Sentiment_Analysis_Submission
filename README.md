# Customer Review Sentiment Analysis 📊🤖

A beginner-friendly **Natural Language Processing (NLP) + Machine Learning** project that analyzes customer reviews and classifies them into **Positive, Negative, or Neutral** sentiments.

This project was developed as part of the **XTRAGRAD AI Internship 2026 – Week 2 Mini AI Assignment**.

---

## 📌 Project Overview

Customer reviews contain valuable information about how people feel about a product or service. Manually analyzing a large number of reviews can be time-consuming.

This project demonstrates a basic **sentiment analysis pipeline** that takes customer review text, preprocesses it, converts the text into numerical features using **TF-IDF**, and uses **Logistic Regression** to classify the sentiment.

The complete process includes text preprocessing, feature extraction, model training, prediction, and performance evaluation.

---

## 🎯 Objective

The objective of this project is to build a simple AI system that predicts whether a customer review is:

* 🟢 **Positive**
* 🔴 **Negative**
* 🟡 **Neutral**

The model's performance is evaluated using **accuracy, confusion matrix, and classification report**.

---

## 🔄 Workflow

```text
Customer Reviews
       ↓
Text Preprocessing
       ↓
TF-IDF Feature Extraction
       ↓
Train-Test Split
       ↓
Logistic Regression
       ↓
Sentiment Prediction
       ↓
Model Evaluation
       ↓
Accuracy + Confusion Matrix + Classification Report
```

---

## 🛠️ Technologies Used

### Programming Language

* **Python**

### Libraries & Tools

* **Pandas**
* **Regular Expressions (`re`)**
* **Scikit-learn**
* **Jupyter Notebook**

### Machine Learning & NLP Techniques

* Text Preprocessing
* TF-IDF Vectorization
* Logistic Regression
* Train-Test Split
* Sentiment Classification
* Accuracy Evaluation
* Confusion Matrix
* Classification Report

---

## 📂 Project Structure

```text
Customer_Review_Sentiment_Analysis_Submission/
│
├── Customer_Review_Sentiment_Analysis.ipynb
├── customer_reviews.csv
├── final_predictions.png
└── README.md
```

### File Description

| File                                       | Description                                                                                |
| ------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `Customer_Review_Sentiment_Analysis.ipynb` | Jupyter Notebook containing data preprocessing, model training, prediction, and evaluation |
| `customer_reviews.csv`                     | Dataset containing customer reviews and their sentiment labels                             |
| `final_predictions.png`                    | Screenshot/image showing the final prediction results                                      |
| `README.md`                                | Project documentation                                                                      |

---

## 📊 Dataset

The project uses a small custom dataset containing **30 customer reviews**.

| Sentiment   | Number of Reviews |
| ----------- | ----------------: |
| 🟢 Positive |                10 |
| 🔴 Negative |                10 |
| 🟡 Neutral  |                10 |
| **Total**   |            **30** |

The dataset contains two columns:

| Column      | Description                                     |
| ----------- | ----------------------------------------------- |
| `review`    | Text of the customer review                     |
| `sentiment` | Sentiment label: Positive, Negative, or Neutral |

---

## 🧹 Text Preprocessing

Before training the machine learning model, the review text is cleaned and prepared.

### Preprocessing Steps

1. Convert text to **lowercase**
2. Remove **non-letter characters**
3. Clean the review text for feature extraction

This preprocessing helps create a more consistent representation of the input text.

---

## 🔢 TF-IDF Feature Extraction

After preprocessing, the text is converted into numerical features using **TF-IDF (Term Frequency-Inverse Document Frequency)**.

TF-IDF assigns importance to words based on:

* How frequently a word appears in a review
* How common or rare the word is across all reviews

This converts textual data into numerical values that can be used by the machine learning model.

---

## 🤖 Machine Learning Model

### Logistic Regression

**Logistic Regression** is used as the classification algorithm.

The model is trained on the TF-IDF features and learns patterns associated with the three sentiment categories:

```text
Positive
Negative
Neutral
```

A **train-test split** is used to separate the data into training and testing sets.

---

## 📈 Model Evaluation

The trained model is evaluated using the following metrics:

### Accuracy

Measures the percentage of correctly classified reviews.

### Confusion Matrix

Shows the number of:

* Correct predictions
* Incorrect predictions
* Misclassifications between sentiment categories

### Classification Report

Provides common classification metrics such as:

* **Precision**
* **Recall**
* **F1-score**

These metrics provide a better understanding of the model's performance for each sentiment class.

---

## 🖼️ Prediction Results

The project includes a screenshot of the final predictions and results:

```text
final_predictions.png
```

The predictions demonstrate how the trained model classifies customer reviews into **Positive, Negative, or Neutral** categories.

---

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/Shivanshbajaj1/Customer_Review_Sentiment_Analysis_Submission.git
```

### 2. Navigate to the Project Directory

```bash
cd Customer_Review_Sentiment_Analysis_Submission
```

### 3. Install Required Libraries

```bash
pip install pandas scikit-learn jupyter
```

### 4. Open the Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Customer_Review_Sentiment_Analysis.ipynb
```

### 5. Run the Notebook

Execute the notebook cells in order to:

* Load the dataset
* Preprocess the reviews
* Generate TF-IDF features
* Train the Logistic Regression model
* Predict sentiments
* Evaluate the model

---

## 📌 Key Learning Outcomes

Through this project, the following concepts were implemented:

* Understanding basic **NLP workflows**
* Cleaning and preprocessing text data
* Converting text into numerical features using **TF-IDF**
* Applying **Logistic Regression** for classification
* Splitting data into training and testing sets
* Evaluating a machine learning classification model
* Understanding confusion matrices and classification reports

---

## 🔮 Future Improvements

The project can be extended by:

* Increasing the dataset size
* Using a larger and more diverse review dataset
* Applying advanced NLP preprocessing
* Comparing multiple machine learning algorithms
* Using **word embeddings** or transformer-based models
* Deploying the model as a web application

---

## 👨‍💻 Author

**Shivansh Bajaj**

GitHub: [Shivanshbajaj1](https://github.com/Shivanshbajaj1)

---

## ⭐ Project

This project was created for learning and demonstrating the fundamentals of **NLP, Machine Learning, and Sentiment Analysis**.

# Customer Review Sentiment Analysis 📊🤖

A beginner-friendly **Natural Language Processing (NLP) + Machine Learning** project that analyzes customer reviews and classifies them into **Positive, Negative, or Neutral** sentiments.

This project was developed as part of the **XTRAGRAD AI Internship 2026 – Week 2 Mini AI Assignment**.

---

## 📌 Project Overview

Customer reviews contain valuable information about how people feel about a product or service. Manually analyzing a large number of reviews can be time-consuming.

This project demonstrates a basic sentiment-analysis pipeline that takes customer review text, preprocesses it, converts it into numerical features using **TF-IDF**, and uses **Logistic Regression** to predict the sentiment.

### 🔄 Workflow

```text
Customer Reviews
       ↓
Text Preprocessing
       ↓
TF-IDF Feature Extraction
       ↓
Logistic Regression
       ↓
Sentiment Prediction
       ↓
Model Evaluation
🎯 Objective

The objective of this project is to build a simple AI system that predicts whether a customer review is:

🟢 Positive
🔴 Negative
🟡 Neutral

The project also evaluates the model's performance using accuracy, confusion matrix, and classification report.

🛠️ Technologies Used
Programming Language
Python
Libraries & Tools
Pandas
Regular Expressions (re)
Scikit-learn
Jupyter Notebook
Machine Learning & NLP Techniques
Text Preprocessing
TF-IDF Vectorization
Logistic Regression
Train-Test Split
Sentiment Classification
Accuracy Evaluation
Confusion Matrix
Classification Report
📂 Project Structure
Customer-Review-Sentiment-Analysis/
│
├── Customer_Review_Sentiment_Analysis.ipynb
├── customer_reviews.csv
├── final_predictions.png
└── README.md
📊 Dataset

The project uses a small custom dataset containing 30 customer reviews.

Sentiment	Number of Reviews
Positive	10
Negative	10
Neutral	10
Total	30

The dataset contains two columns:

review
sentiment
🧹 Text Preprocessing

The review text is cleaned before training the machine learning model.

Preprocessing Steps
Converting text to lowercase
Removing non-letter characters
Removing extra spaces
Example

Original Review:

"The Product Is AMAZING!!!"

After Preprocessing:

"the product is amazing"
🔢 TF-IDF Feature Extraction

TF-IDF (Term Frequency-Inverse Document Frequency) is used to convert text into numerical feature vectors that can be processed by the machine learning model.

TF-IDF gives higher importance to words that are useful for distinguishing documents while reducing the importance of words that appear very commonly across documents.

In this project, the TF-IDF vectorizer is fitted only on the training data and then used to transform the test data.

This approach helps prevent information from the test set from leaking into the training process.

🤖 Machine Learning Model
Logistic Regression

The project uses Logistic Regression as the classification model.

Logistic Regression was selected as a simple baseline model for text classification when combined with TF-IDF features.

model = LogisticRegression(max_iter=1000)
model.fit(X_train_tfidf, y_train)
🧪 Train-Test Split

The dataset is divided into:

80% Training Data
20% Testing Data

A fixed random state is used for reproducibility.

train_test_split(
    X,
    y,
    test_size=0.20,
    random_state=42,
    stratify=y
)

The use of stratify=y helps maintain the class distribution between the training and testing sets.

📈 Results

The trained model achieved:

Test Accuracy

50.00%

The model was evaluated using:

Accuracy
Confusion Matrix
Classification Report

Because the dataset contains only 30 reviews, the results should be considered a basic educational demonstration rather than a production-level sentiment-analysis system.

🔍 Testing on New Reviews

The trained model was also tested on three new customer reviews.

Customer Review	Prediction
Amazing product and fast delivery!	Positive
The quality is terrible and disappointing.	Negative
The package arrived today.	Neutral

These examples demonstrate how the trained model can be used to predict sentiment for previously unseen text.

💡 Example Use Cases

Sentiment analysis can help companies:

Monitor customer feedback
Identify negative customer experiences
Measure customer satisfaction
Analyze product reviews
Summarize large amounts of textual feedback
📚 Key Learning Outcomes

Through this project, I learned how to:

Work with textual datasets
Perform basic text preprocessing
Apply NLP techniques to machine learning
Convert text into numerical features using TF-IDF
Train a classification model
Generate sentiment predictions
Evaluate machine learning performance
Understand the limitations of small datasets
⚠️ Limitations

This project is intentionally simple and has several limitations:

Very small dataset of only 30 reviews
Basic text preprocessing
Limited training examples for each sentiment
No advanced NLP techniques
Model performance may vary with new types of reviews

A larger and more diverse dataset would be required to build a more reliable real-world sentiment-analysis system.

🚀 Future Improvements

Possible improvements include:

Using a much larger and more diverse dataset
Adding stopword removal and lemmatization
Trying models such as SVM, Random Forest, or Naive Bayes
Hyperparameter tuning
Using word embeddings
Experimenting with transformer-based models
Creating a Streamlit web interface
Deploying the sentiment-analysis system online
📝 Assignment Questions
1. What is Sentiment Analysis?

Sentiment analysis is the process of analyzing text and identifying the opinion or emotional tone expressed in it.

In this project, customer reviews are classified into Positive, Negative, or Neutral categories.

2. Why is Sentiment Analysis useful for companies?

Companies can automatically analyze large numbers of customer reviews to identify positive feedback, negative experiences, and neutral comments.

This can help them understand customer opinions and monitor feedback more efficiently.

3. What is NLP?

Natural Language Processing (NLP) is a field of Artificial Intelligence that enables computers to process, analyze, and understand human language.

4. What is TF-IDF?

TF-IDF stands for Term Frequency-Inverse Document Frequency.

It is a technique used to convert text into numerical features while giving importance to words that help distinguish one document from another.

5. Which model was used?

Logistic Regression was used as the machine learning classification model for sentiment prediction.

6. What accuracy was achieved?

The model achieved 50.00% accuracy on the held-out test set.

👨‍💻 Author

Shivansh Bajaj

B.Tech CSE (AI & ML)

📜 Internship

This project was completed as part of the:

XTRAGRAD AI Internship 2026 – Foundation Track

Week 2 Mini AI Assignment

Internship Start Date: 1 September 2026

⭐ Project Highlights
Beginner-friendly NLP project
Text classification using machine learning
TF-IDF based feature extraction
Logistic Regression classifier
Positive / Negative / Neutral sentiment prediction
Model evaluation using standard metrics
Built as part of the XTRAGRAD AI Internship 2026

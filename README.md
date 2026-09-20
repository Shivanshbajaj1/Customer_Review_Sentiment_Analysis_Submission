# Customer Review Sentiment Analysis 📊🤖

A beginner-friendly **Natural Language Processing (NLP) + Machine Learning** project that analyzes customer reviews and classifies them into **Positive, Negative, or Neutral** sentiments.

This project was developed as part of the **XTRAGRAD AI Internship 2026 – Mini AI Assignment**.

---

## 📌 Project Overview

Customer reviews contain valuable information about how people feel about a product or service. Manually analyzing a large number of reviews can be time-consuming.

This project demonstrates a basic sentiment-analysis pipeline that takes customer review text, preprocesses it, converts it into numerical features using **TF-IDF**, and uses **Logistic Regression** to predict the sentiment.

### Workflow

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

Build a simple AI system that predicts whether a customer review is:

Positive
Negative
Neutral

The project also evaluates the model's performance using accuracy, confusion matrix, and classification report.

🛠️ Technologies Used
Python
Pandas
Regular Expressions (re)
Scikit-learn
Jupyter Notebook
Machine Learning Techniques
Text preprocessing
TF-IDF Vectorization
Logistic Regression
Train/Test Split
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

The review text is cleaned before training the model.

The preprocessing steps include:

Converting text to lowercase
Removing non-letter characters
Removing extra spaces

Example:

"The Product Is AMAZING!!!"

becomes:

"the product is amazing"
🔢 TF-IDF Feature Extraction

TF-IDF (Term Frequency-Inverse Document Frequency) is used to convert text into numerical feature vectors.

It gives higher importance to words that are useful for distinguishing between documents while reducing the importance of very common words.

The TF-IDF vectorizer is fitted only on the training data and then used to transform the test data.

🤖 Machine Learning Model
Logistic Regression

The project uses Logistic Regression as the classification model.

It was selected because it is a simple and effective baseline model for text classification when combined with TF-IDF features.

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
📈 Results

The model achieved:

Test Accuracy: 50.00%

The model was evaluated using:

Accuracy
Confusion Matrix
Classification Report

Because the dataset contains only 30 reviews, the results should be considered a basic demonstration rather than a production-level sentiment-analysis system.

🔍 Testing on New Reviews

The trained model was also tested on three new reviews:

Customer Review	Prediction
Amazing product and fast delivery!	Positive
The quality is terrible and disappointing.	Negative
The package arrived today.	Neutral

These examples demonstrate how the trained model can be used to predict sentiment for previously unseen text.

💡 Example Use Cases

Sentiment analysis can help companies:

Monitor customer feedback
Identify negative experiences
Measure customer satisfaction
Analyze product reviews
Summarize large amounts of textual feedback
📚 Key Learning Outcomes

Through this project, I learned how to:

Work with textual datasets
Perform basic text preprocessing
Use NLP techniques for machine learning
Convert text into numerical features using TF-IDF
Train a classification model
Generate sentiment predictions
Evaluate machine learning performance
Understand the limitations of small datasets
⚠️ Limitations

This project is intentionally simple and has several limitations:

Very small dataset of only 30 reviews
Basic text preprocessing
No advanced NLP techniques
Limited training examples for each sentiment
Model performance may vary with new types of reviews

A larger and more diverse dataset would be required for a more reliable real-world system.

🚀 Future Improvements

Possible improvements include:

Using a much larger dataset
Adding stopword removal and lemmatization
Trying models such as SVM, Random Forest, or Naive Bayes
Hyperparameter tuning
Using word embeddings
Experimenting with transformer-based models
Creating a Streamlit web interface
Deploying the sentiment-analysis system online
📝 Assignment Questions
1. What is Sentiment Analysis?

Sentiment analysis is the process of analyzing text and identifying the opinion or emotional tone expressed in it. In this project, reviews are classified as Positive, Negative, or Neutral.

2. Why is Sentiment Analysis useful for companies?

Companies can automatically analyze large numbers of customer reviews to identify positive feedback, negative experiences, and neutral comments.

3. What is NLP?

Natural Language Processing (NLP) is a field of Artificial Intelligence that enables computers to process and understand human language.

4. What is TF-IDF?

TF-IDF stands for Term Frequency-Inverse Document Frequency. It converts text into numerical features and gives importance to terms that help distinguish documents.

5. Which model was used?

Logistic Regression was used as a basic classification model for sentiment prediction.

6. What accuracy was achieved?

The model achieved 50.00% accuracy on the held-out test set.

👨‍💻 Author

Shivansh Bajaj

B.Tech CSE (AI & ML)

📜 Internship

This project was completed as part of the:

XTRAGRAD AI Internship 2026 – Foundation Track

Internship start date: 1 September 2026

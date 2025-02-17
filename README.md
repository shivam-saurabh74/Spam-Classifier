# Spam-Classifier
This project is an SMS spam detection system using machine learning. The system classifies SMS messages into two categories: Ham (non-spam) and Spam. The goal is to use various machine learning algorithms to build an accurate classifier for identifying spam messages.
#Project Overview
This project involves:
  Loading and cleaning a dataset of SMS messages.
  Preprocessing the text data (including tokenization, stop-word removal, and stemming).
  Vectorizing the text using TF-IDF.
  Building and evaluating different machine learning models to classify the messages as ham (non-spam) or spam.
  Allowing the user to input a message and classify it as spam or ham.
#Dataset
The dataset used in this project is the SMS Spam Collection dataset, which contains 5,572 SMS messages labeled as spam or ham. It can be found https://archive.ics.uci.edu/dataset/228/sms+spam+collection .

#Key Steps
1. Data Loading and Cleaning
The dataset is loaded from a CSV file.
Unnecessary columns are removed, and the remaining columns are renamed for clarity.
Target values (ham or spam) are encoded into numeric values using LabelEncoder.
2. Exploratory Data Analysis (EDA)
Basic exploration of the dataset is done to understand its structure.
A pie chart visualizes the distribution of spam and ham messages.
Basic text statistics such as the number of characters, words, and sentences are calculated.
3. Text Preprocessing
Text is cleaned by:
Converting to lowercase
Tokenizing the text
Removing special characters, stop words, and punctuation
Stemming the words
4. Text Vectorization
The text is converted into numerical vectors using TF-IDF (Term Frequency-Inverse Document Frequency).
5. Model Building and Evaluation
Several machine learning algorithms are tested, including:
Naive Bayes (Gaussian, Multinomial, Bernoulli)
Support Vector Classifier (SVC)
Logistic Regression
Random Forest
K-Nearest Neighbors (KNN)
AdaBoost, Bagging, Extra Trees, Gradient Boosting, and XGBoost
Models are evaluated using accuracy and precision metrics.
The Multinomial Naive Bayes (MNB) model performs best.
6. User Input Interface
A simple function allows users to input an SMS message and classify it as spam or ham using the trained model.

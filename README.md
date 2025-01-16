# Depression Detection from Social Media Posts using Machine Learning

## Introduction
This project aims to develop a machine learning model capable of detecting depressive content in Reddit posts. By analyzing text data from various subreddits, we aim to distinguish between depressive and non-depressive content, potentially aiding in early detection and intervention for individuals experiencing depression.

## Problem Statement
Depression is a leading cause of mental ill-health and significantly increases the risk of early death. Unfortunately, 70% of individuals experiencing depression do not seek medical consultation. With the growing reliance on social media for expressing emotions and daily life activities, analyzing this data offers a valuable opportunity to detect mental health issues. This project applies machine learning techniques to social media data, focusing on depression detection.

---

## Features of the Project

### 1. Data Collection
- **Method:** Utilized the AsyncPRAW library to asynchronously interact with Reddit's API.
- **Purpose:** Gather data from depressive and non-depressive subreddits to create a balanced dataset.
- **Efficiency:** Asynchronous programming reduced data collection time by handling multiple API requests concurrently.

### 2. Data Preprocessing
Text preprocessing techniques were employed to clean and standardize the data:
- Converted text to lowercase.
- Removed URLs and non-alphabetic characters.
- Tokenized text into individual words.
- Removed stop words to focus on meaningful content.
- Applied lemmatization to normalize words to their base form.

### 3. Exploratory Data Analysis (EDA)
EDA helped uncover patterns and biases in the dataset:
- Analyzed dataset attributes such as shape and null values.
- Evaluated text length statistics and detected outliers.
- Created visualizations, including label distribution, text length distribution, and word clouds.

### 4. Feature Extraction
- **Technique:** TF-IDF (Term Frequency-Inverse Document Frequency) vectorization.
- **Purpose:** Convert text data into numerical features while capturing the contextual importance of words.

### 5. Model Training and Evaluation
Trained and evaluated multiple machine learning models:
- Logistic Regression (baseline model).
- K-Nearest Neighbors (local pattern capture).
- Decision Tree (non-linear decision boundaries).
- Support Vector Machine (high-dimensional data handling).
- Naive Bayes (efficient for text classification).
- Multi-Layer Perceptron (complex pattern recognition).

Additionally, ensemble methods (Voting Classifier and Blending Classifier) were implemented to improve overall model accuracy.

### 6. Main Execution Flow
The process is orchestrated through a main function:
1. Data Collection
2. Preprocessing
3. Exploratory Data Analysis
4. Feature Extraction
5. Model Training and Evaluation

Asynchronous execution is utilized to enhance the efficiency of the data collection process.

---

## Technologies and Libraries Used
1. **AsyncPRAW:** Efficiently handles asynchronous API requests for large-scale data collection.
2. **Pandas:** For data manipulation and analysis.
3. **NLTK:** Provides tools for text preprocessing, including tokenization and lemmatization.
4. **Scikit-learn:** Offers various machine learning algorithms and tools for feature extraction, model training, and evaluation.
5. **Matplotlib & Seaborn:** Used for creating visualizations during EDA.
6. **WordCloud:** Provides intuitive visual representations of the most frequent words.

---

## Conclusion
This project demonstrates the potential of machine learning in detecting depressive content from social media posts. By leveraging NLP techniques and multiple machine learning models, the system achieved reasonable accuracy in distinguishing depressive and non-depressive content. While promising, this tool should be used in conjunction with professional medical advice for mental health assessment and intervention.

---

## Team Members and Roles
- **Soumya Kumari (22322027)**
- **Lavisha Kapoor (22112061)**
- **Kanishka Soni (22112050)**

**Roles:** All team members contributed equally to the project's development.


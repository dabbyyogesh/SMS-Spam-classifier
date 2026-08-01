# ✉️ SMS & Email Spam Classifier

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![NLP](https://img.shields.io/badge/NLP-NLTK-green)
![Deployment](https://img.shields.io/badge/Deployment-Streamlit-red)

## 📌 Overview
This is an end-to-end Machine Learning and Natural Language Processing (NLP) web application that classifies SMS messages and emails as either **Spam** or **Ham** (Normal). The model is optimized for high precision to ensure that legitimate messages are not incorrectly flagged as spam. 

🌐 **Live Demo:** [Insert your Live App Link Here]

## 🚀 Features
* **Interactive UI:** A clean, easy-to-use web interface built with Streamlit.
* **Real-Time Prediction:** Instantly analyzes user-inputted text and returns a Spam/Ham classification.
* **Robust NLP Pipeline:** Handles lowercasing, tokenization, stop-word removal, punctuation stripping, and word stemming.

## 🧠 Project Pipeline
1. **Data Cleaning & EDA:** Removed duplicates and null values. Visualized character, word, and sentence distributions using Matplotlib and Seaborn. Generated WordClouds to identify the most frequent terms in spam vs. ham messages.
2. **Text Preprocessing:** Utilized `NLTK` to clean the raw text. Converted words to their root forms using the `PorterStemmer`.
3. **Vectorization:** Transformed the cleaned text into numerical vectors using `TF-IDF Vectorizer` (Term Frequency-Inverse Document Frequency).
4. **Model Training:** Tested multiple algorithms (Support Vector Machines, Random Forests, etc.). Selected **Multinomial Naive Bayes** as the final model due to its superior Precision score in text classification.
5. **Deployment:** Exported the trained model and vectorizer using `pickle` and deployed the application to the web using Streamlit Community Cloud.

## 🛠️ Technologies Used
* **Programming Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn
* **Natural Language Processing:** NLTK
* **Data Visualization:** Matplotlib, Seaborn, WordCloud
* **Web Framework:** Streamlit

## 📂 Repository Structure
* `app.py`: The main Streamlit application script.
* `model.pkl`: The trained Multinomial Naive Bayes machine learning model.
* `vectorizer.pkl`: The fitted TF-IDF vectorizer used to transform input text.
* `requirements.txt`: The list of Python dependencies required to run the app.
* `spam_calssification_v2.ipynb`: The Jupyter Notebook containing the full data analysis, preprocessing, and model training workflow.
* `spam.csv`: The dataset used to train the model.

## 💻 How to Run Locally
just open this link in your browser

https://wbg5bvsfbgrrub22u6ygcu.streamlit.app/

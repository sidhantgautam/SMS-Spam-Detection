
# 📨 SMS Spam Classification using Machine Learning

## 🚀 Project Overview
This project is a complete solution to detect whether an SMS message is **Spam** or **Ham (Not Spam)** using various Machine Learning algorithms.  
It covers the entire pipeline from **data cleaning**, **exploratory data analysis (EDA)**, **text preprocessing**, to **model building**, **evaluation**, and **deployment preparation**.

---

## ✅ Key Features

1. **Data Cleaning**  
   - Removed irrelevant columns  
   - Handled missing and duplicate data  
   - Encoded target labels (Ham → 0, Spam → 1)

2. **Exploratory Data Analysis (EDA)**  
   - Visualized data distribution  
   - Studied message length, number of words, and sentences  
   - Identified class imbalance  
   - Created Word Clouds for Spam and Ham messages  
   - Visualized most frequent words in Spam and Ham

3. **Text Preprocessing**  
   - Lowercased text  
   - Tokenization  
   - Removed stop words and special characters  
   - Applied Stemming

4. **Feature Extraction**  
   - Used **TF-IDF Vectorizer**  
   - Appended additional features like the number of characters

5. **Model Building & Evaluation**  
   - Tested multiple models:  
     - Support Vector Classifier (SVC)  
     - K-Nearest Neighbors (KNN)  
     - Naive Bayes (Multinomial & Bernoulli)  
     - Decision Tree  
     - Random Forest  
     - AdaBoost  
     - Bagging  
     - Extra Trees Classifier (ETC)  
     - Gradient Boosting Decision Trees (GBDT)  
     - XGBoost  
   - Evaluated based on **Accuracy** and **Precision**

6. **Model Improvement**  
   - Optimized TF-IDF parameters  
   - Applied feature scaling  
   - Experimented with adding extra features (e.g., number of characters)

7. **Ensemble Learning**  
   - Applied **Voting Classifier** combining SVC, Naive Bayes, and Extra Trees  
   - Applied **Stacking Classifier** with Random Forest as final estimator  
   - Achieved top performance with high accuracy and precision

8. **Model Export**  
   - Saved the trained **TF-IDF Vectorizer** and **Naive Bayes model** using Pickle for later use in deployment

---

## 📊 Performance Summary

| Algorithm            | Accuracy | Precision |
|----------------------|----------|-----------|
| Extra Trees Classifier | ~0.9778  | ~0.9915  |
| Random Forest         | ~0.9700  | ~0.9908  |
| Voting Classifier     | ~0.9816  | ~0.9917  |
| Stacking Classifier   | ~0.9787  | ~0.9328  |
| Multinomial NB        | ~0.9594  | 1.0000   |

---

## ⚙️ How To Use

1. Clone the repository:  
   ```bash
   git clone https://github.com/sidhantgautam/SMS-Spam-Detection.git
   cd sms-spam-classification
   ```

2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook `SMS_Spam_Classification.ipynb` in Google Colab or locally to explore the entire workflow.

4. For Deployment:  
   Load the saved `vectorizer.pkl` and `model.pkl` to make predictions on new SMS messages.

---

## 📚 Dependencies

- Python ≥ 3.7  
- scikit-learn  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- nltk  
- wordcloud  
- xgboost

---

## 💡 Future Work

- Improve preprocessing with advanced NLP techniques (e.g., lemmatization)  
- Hyperparameter tuning for optimal model performance  
- Build a simple web interface for real-time spam detection using Flask or FastAPI

---



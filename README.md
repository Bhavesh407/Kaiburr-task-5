# Kaiburr Assessment - Task 5: Data Science (Text Classification)

This project involves performing text classification on the Consumer Complaint Database. The goal is to build, train, and evaluate a machine learning model that can classify consumer complaints into one of four categories, as required by the assessment:
* 0: "Credit reporting, repair, or other"
* 1: "Debt collection"
* 2: "Consumer Loan"
* 3: "Mortgage"

---

## Process Overview

The project was completed using Python in a Google Colab notebook.

1.  **Explanatory Data Analysis (EDA):** The dataset (`complaints.csv`) was loaded from Google Drive. It was filtered to keep only the four required product categories and to remove any complaints that had no narrative text.
2.  **Text Pre-Processing:** A function was created to clean the complaint text. This process involved converting text to lowercase, removing all punctuation and numbers, and filtering out common English "stop words" (like 'the', 'is', 'at').
3.  **Feature Engineering:** The cleaned text was converted into numerical features using `TfidfVectorizer`, which represents the importance of each word in the text. The data was then split into a training set (80%) and a testing set (20%).
4.  **Model Selection & Comparison:** Two different multi-class classification models were trained:
    * **Logistic Regression**
    * **Multinomial Naive Bayes**
5.  **Model Evaluation:** The Logistic Regression model performed better (96.98% accuracy) and was selected as the final model. A detailed classification report was generated to evaluate its performance on precision, recall, and f1-score for each category.
6.  **Prediction:** The trained model was successfully used to predict the category of a new, unseen complaint ("I was overcharged on my mortgage payment..."), which it correctly classified as "Mortgage".

---

## Screenshots of Results

**Note:** All screenshots include my device name ("Bhavesh-Dell-G15") and the system date/time, as required.

### 1. Data Loading and EDA
<img width="1918" height="1078" alt="1" src="https://github.com/user-attachments/assets/e4c41949-c065-47f1-8885-3157cc2ea3ab" />
<img width="1918" height="1078" alt="2" src="https://github.com/user-attachments/assets/9372c63d-ea3b-4732-a969-c084e24881a6" />

### 2. Text Pre-Processing
<img width="1918" height="1078" alt="3" src="https://github.com/user-attachments/assets/779a6e04-7abb-462a-a39e-6a9eb70c6779" />

### 3. Model Comparison
<img width="1918" height="1078" alt="4" src="https://github.com/user-attachments/assets/c81295bb-d0ca-46b8-8623-566a94bf65d2" />

### 4. Final Model Evaluation
<img width="1918" height="1078" alt="5" src="https://github.com/user-attachments/assets/7771d21f-54b0-4510-a7e0-bd5947212895" />

### 5. Final Prediction
<img width="1918" height="1078" alt="6" src="https://github.com/user-attachments/assets/a1b47367-93eb-4294-bb9a-1332a787d0e5" />

Spam SMS Detection using Machine Learning
Project Overview

This project aims to classify SMS messages as Spam or Ham (Legitimate) using Machine Learning techniques. The model is trained on a dataset of SMS messages and uses TF-IDF Vectorization for feature extraction along with a Naive Bayes Classifier for prediction.

Objective

The objective of this project is to automatically identify unwanted spam messages and distinguish them from legitimate SMS messages.

Dataset

The dataset contains SMS messages labeled as:

Ham (0): Legitimate messages
Spam (1): Unwanted promotional or fraudulent messages
Technologies Used
Python
Google Colab
Pandas
NumPy
Scikit-learn
TF-IDF Vectorizer
Multinomial Naive Bayes
Project Workflow
1. Data Collection
Loaded the SMS Spam Collection dataset.
2. Data Preprocessing
Removed unnecessary columns.
Renamed columns for better understanding.
Converted labels:
Ham → 0
Spam → 1
3. Feature Extraction
Applied TF-IDF (Term Frequency-Inverse Document Frequency) to convert text messages into numerical vectors.
4. Data Splitting
Split the dataset into:
80% Training Data
20% Testing Data
5. Model Training
Trained a Multinomial Naive Bayes classifier on the TF-IDF features.
6. Model Evaluation
Evaluated the model using:
Accuracy Score
Precision
Recall
F1-Score
Confusion Matrix
7. Prediction
Built a function to predict whether a new SMS message is Spam or Ham.
Results
Achieved high accuracy in classifying SMS messages.
Successfully identified spam and legitimate messages with good precision and recall.
Sample Predictions
SMS Message	Prediction
Congratulations! You have won a free iPhone.	Spam
Hi, are we meeting tomorrow?	Ham
Claim your reward now by clicking the link.	Spam
Please send me the notes after class.	Ham
Future Enhancements
Implement Support Vector Machine (SVM) for improved performance.
Deploy the model as a web application using Flask.
Integrate real-time SMS classification.
Compare multiple machine learning algorithms.
How to Run the Project
Install Required Libraries
pip install pandas numpy scikit-learn
Run the Notebook
Spam_SMS_Detection.ipynb
Train the Model
model.fit(X_train_tfidf, y_train)
Predict New Messages
predict_sms("Congratulations! You have won a free iPhone")
Project Structure
Spam-SMS-Detection/
│
├── Spam_SMS_Detection.ipynb
├── spam.csv
├── spam_model.pkl
├── tfidf.pkl
└── README.md
Conclusion

The Spam SMS Detection system effectively classifies SMS messages as spam or legitimate using TF-IDF and Naive Bayes. This project demonstrates the practical application of Natural Language Processing (NLP) and Machine Learning in detecting unwanted messages and improving communication security.


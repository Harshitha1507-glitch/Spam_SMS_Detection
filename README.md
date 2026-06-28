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

3. Data Preprocessing

	Removed unnecessary columns.
	Renamed columns for better understanding.
	Converted labels:
	Ham → 0
	Spam → 1

5. Feature Extraction
   
	Applied TF-IDF (Term Frequency-Inverse Document Frequency) to convert text messages into numerical vectors.

7. Data Splitting

	Split the dataset into:
	80% Training Data
	20% Testing Data

9. Model Training
    
	Trained a Multinomial Naive Bayes classifier on the TF-IDF features.

11. Model Evaluation
    
	Evaluated the model using:
	Accuracy Score
	Precision
	Recall
	F1-Score
	Confusion Matrix

13. Prediction
    
	Built a function to predict whether a new SMS message is Spam or Ham.

Results

Achieved high accuracy in classifying SMS messages.
Successfully identified spam and legitimate messages with good precision and recall.

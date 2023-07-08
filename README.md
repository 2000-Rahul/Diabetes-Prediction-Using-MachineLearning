## Diabetes Prediction Using Machine Learning
- **Machine learning** is a growing technology which enables computers to learn automatically from past data. Machine learning uses various algorithms for building mathematical      models and making predictions using historical data or information. Currently, it is being used for various tasks such as image recognition, speech recognition, email            filtering, Facebook auto-tagging, recommender system, and many more.

## Overview of model
- In this model, we will be predicting that whether the patient has diabetes or not on the basis of the features we will provide to our machine learning model.
- In this model **SVM** algorithm is used for prediction of diabetes patient.
- Support Vector Machine or SVM is one of the most popular Supervised Learning algorithms, which is used for Classification as well as Regression problems. However, primarily,     it is used for Classification problems in Machine Learning.

## Model building

**Importing libraries** <br>
 - **Numpy** : NumPy stands for Numerical Python. NumPy is a Python library used for working with arrays.It also has functions for working in domain of linear algebra, fourier                  transform, and matrices.NumPy was created in 2005 by Travis Oliphant. It is an open source project and you can use it freely. <br>

 - **Pandas** : Pandas is a Python library used for working with data sets.It has functions for analyzing, cleaning, exploring, and manipulating data.The name "Pandas" has a                     reference to both "Panel Data", and "Python Data Analysis" and was created by Wes McKinney in 2008.

## Performing Exploratory Data Analysis (EDA) 
- Exploratory Data Analysis (EDA) is a crucial step in data analysis. It helps to understand the nature of the data and identify any patterns or trends hidden within it. We can    gain insights into the data using various visualization techniques and statistical methods, which can help make informed decisions. <br>
          In this model I have covered some essential techniques for performing EDA, such as summary statistics.

## Scikit-learn
- It is an open source data analysis library, and the gold standard for Machine Learning (ML) in the Python ecosystem. Key concepts and features include:                           Algorithmic decision-making methods, including: Classification: identifying and categorizing data based on patterns. <br>

- **from sklearn.preprocessing import StandardScaler** <br>

  **StandardScaler**: The StandardScaler function of sklearn is based on the theory that the dataset's variables whose values lie in different ranges do not have an equal                              contribution to the model's fit parameters and training function and may even lead to bias in the predictions made with that model. Therefore, before                             including the features in the machine learning model, we must normalize the data (µ = 0, σ = 1). Standardization in feature engineering is commonly                               employed to address this potential issue.

- **sklearn.model_selection.train_test_split() function** <br>
  The train_test_split() method is used to split our data into train and test sets. First, we need to divide our data into features (X) and labels (y). The dataframe gets          divided into X_train, X_test, y_train, and y_test. X_train and y_train sets are used for training and fitting the model. The X_test and y_test sets are used for testing the      model if it’s predicting the right outputs/labels. we can explicitly test the size of the train and test sets. It is suggested to keep our train sets larger than the test sets

- **from sklearn import svm** <br>
  Support vector machines (SVMs) are a set of supervised learning algorithm used for classification, regression and outliers detection.

- **from sklearn.metrics import accuracy_score** <br>
  Accuracy classification score. <br>
  In multilabel classification, this function computes subset accuracy: the set of labels predicted for a sample must exactly match the corresponding set of labels in y_true.

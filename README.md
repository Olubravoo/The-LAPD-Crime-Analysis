**LAPD Crime Dataset Analysis and Classification**

**Project Overview**

This project focuses on analyzing historical crime incident data from the Los Angeles Police Department (LAPD) to build a predictive machine learning model. Instead of traditional 
time-series forecasting, this project utilizes classification techniques to predict crime-related outcomes based on environmental, temporal, and geographic features.

The workflow transitions from initial data exploration and preprocessing to training a robust ensemble classifier, providing a framework that can support law enforcement resource allocation and data-driven public safety strategies.

**Key Components**

**Data Preprocessing & Feature Engineering**

Raw LAPD incident data is cleaned and structured for machine learning:

•	Feature Encoding: Categorical variables are converted into numerical formats using LabelEncoder to make them compatible with the model.

•	Feature Scaling: Continuous numeric features are normalized using StandardScaler to ensure uniform feature scale and improve algorithm convergence.

•	Dataset Splitting: The data is divided into independent variables ($X$) and the dependent target variable ($y$), then partitioned into training and testing sets using train_test_split.

**Predictive Modeling**

The project implements a Random Forest Classifier, an ensemble learning method that operates by constructing a multitude of decision trees during training.
It is chosen for its:

•	High accuracy and resistance to overfitting.

•	Ability to handle complex interactions between categorical and numerical features.

•	Out-of-the-box capability to evaluate feature importance.

**Model Evaluation**

The model's predictive performance is thoroughly evaluated on unseen test data using multiple metrics:

•	Accuracy Score: To measure overall correctness.

•	Confusion Matrix: To visualize true positives, true negatives, false positives, and false negatives.

•	Classification Report: To break down precision, recall, and F1-score for each predicted class.

**Technical Implementation**

The analysis is performed in Python within a Jupyter Notebook environment using the following core libraries:

•	pandas – For data manipulation, cleaning, and structured analysis.

•	numpy – For optimized numerical operations.

•	scikit-learn – For data preprocessing, model training, and evaluation metrics.

•	matplotlib / seaborn – For data exploration and performance visualization.

**Methodology**

1.	Data Loading & Exploration: Import the LAPD dataset and analyze feature distributions.
2.	Preprocessing: Encode categorical data, isolate the target variable, and scale features.
3.	Train-Test Split: Divide the processed dataset into training and validation subsets.
4.	Model Training: Fit a RandomForestClassifier to the training data.
5.	Evaluation: Run predictions on the test set and print the classification metrics to evaluate performance.

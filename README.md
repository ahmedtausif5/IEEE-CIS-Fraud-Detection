# IEEE-CIS-Fraud-Detection

## Authors

#### Tausif Ahmed
#### Mujibul Islam Dipto

## Goal
Detect fraudulent credit card transactions using Machine Learning (ML).

An ML model has been trained using [Vesta's](https://www.vesta.io/) real-world e-commerce transactions for this purpose.


## Outcome
Achieved an accuracy of 87% in detecting fraudulent transactions in the [Kaggle](https://www.kaggle.com/c/ieee-fraud-detection) submission portal.

## Procedure

### Step 0: Data Preparation
* Downcast numerical data types from 64 bit to 32 bit (wherever applicable) to save memory
### Step 1: Explanatory Data Analysis (EDA)
* Explore the features of the dataset, data types of the features, shape of the dataset and so on
* Examine the categorical columns and numerical columns 
* Compute the  number of null values for each columns
* Replace the names of the features in the test set as it was inconsistent with the names of the columns in the training set
* Compare correlations between the features
* Compare the distribution of the target variables
### Step 2: Data Cleansing
* Handle features with missing values
* Convert categorical data to numerical encoding
### Step 3: Model Training Preparation
* Scale the dataset 
* Create train-test split
### Step 4: Data Augmentation
**Aim**: Minimise the adverse effect of skewed data. The given dataset contained significantly greater number of valid transactions compared to the fradulent ones. Data augmentation has been done to balance the target data distribution.
* Under-sample valid transaction data
* Over-sample fraudulent transaction data using SMOTE
### Step 5: Feature Reduction
* Apply PCA to examine the importance of each feature. The amount of variance retained by each has been observed to determine the optimal number of features. 
### Step 6: Application of Classifier
* Apply Random-Forest classifier 
* Calculate evaluation metrics (Accuracy, Precision, Recall, F1 Score)
* Create and plot confusion matrix
* Calculate AUC Score and plot ROC curve
* Predict on test set
* Prepare CSV file for Kaggle submission

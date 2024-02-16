
# Breast Cancer Prediction

This is a survey style project attempting to predict the presence of breast cancer from a number of measurements. In order for our prediction to be efficient we implemented many styles of predictive classifying models. The reason I chose this project was due to the fact how crucial it is to detect any cancer early on in order for treatement to have the biggest effect. Machine learning models will be able to provide consistent faster data than humans can and eliminate human errors. The main focus of our model is to prioritize true positives in order to ensure that fewer serious cases will go unnoticed. Overall it is helpful for machines to detect breast cancer by saving time and money and could ultimately save lives.



## Models Used

Some models that were used were:
* Decision Trees
* Support Machine Vector Classifier
* Logistic Regression
* K-Nearest Neighbors
* Random Forest Classifer


## Dataset Information and Use

The dataset comes from kaggle and provides an ID number to each patient, although we do not require such information so we remove it as we preprocess the data. In order to use the data I first load it into my Pandas dataframe and dropped said ID column and the 'unnamed 32' column. The next step was to turn malignant or benign into 1 being malignant and 0 being benign. Afterwards I  split the data using StandardScaler in order to use the SVM model which is sensitive to range of data.
## Results

The results displayed at the bottom show that the SVM classifier yields the best output in all metrics which shows it is the most suitable in this case. However logistic regression is the next closest in terms of recall which means it could be a good secondary model to use in order to double check while minimizing false negatives if the user chooses to do so. Although the SVM classifier displayed great results we strive for the best to provide the most accurate prediction for our patients!
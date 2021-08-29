# miniprojects
Patient_showup.ipynb
1.	Input data used - patients.csv - appointments.csv
2.	Data was inner joined using patient_id and id columns using merge command.
3.	Checked resulting table for missing values. None was found.
4.	In order to predict whether a person would show up or not, several models were built. But prior to that, data exploration was conducted.
5.	Status variable was the target and it was converted into numeric 
6.	There were 2999897 unique patients in the data. 3 patients had more than 1 appointment. 30% did not show up
7.	Target variable was separated from predictor variables.
8.	Correlation matrix was built using seaborn package to ensure that there are no more high correlations.
9.	Age had a fair amount of positive correlation with hypertension.
10.	Variables were scaled using StandardScaler since it is least affected by outliers.
11.	I tried different modeling algorithms from sklearn - logistic regression, polynomial regression with degree 2, Random Forest, MLP Neural Networks, Decision Tree
12.	Decision tree feature importance shows that age_group is the most important variable followed by sms_reminder.
13.	ROC curves were used to evaluate these algorithms and all models have almost the same accuracy.
14.	Since the model doesn't fit the data very well, we would need to identify additional variables that could help increase the accuracy.

SVM_IRIS_CLASSIFICATION.ipynb
1.	This is an example to showcase models that can predict a classification using Support  vector machines
2.	The code uses the classic IRIS dataset
3.	The data has details on 3 different species – Iris setosa, iris virginica, iris versicolor
4.	The data set consists of 50 samples from each of three species of Iris (Iris setosa, Iris virginica and Iris versicolor), so 150 total samples. Four features were measured from each sample: the length and the width of the sepals and petals, in centimeters.
5.	Before building a model we do some data exploration to see how the data is distributed.
6.	Based on the scatter plot we see Setosa seems the most easily separable
7.	We build a SVM model using the SVC function and the model results are very good
8.	We then try to use a gridsearch to see if the model can be tuned better
9.	The gridsearch seems to be overfitting the model so we will be using results of our previous model
OCR-TESSERACT.ipynb
1.	This project tends to showcase how we can do OCR using tesseract engine 
2.	OCR has varied purposes – OCR is the root of computer vision/object detection etc in images that we see today
3.	In this example I am trying to read a image (that is a user filled out form) and try to read the texts entered by the user into our system
4.	Though OCR is only the first step there are many additional techniques that can be used in order to better the OCR  results
5.	Like annotation is a very useful method where we can label different sections of a  document and retrieve those OCR results pertaining to those sections
6.	And we can build neural net models on top of it to train the model on how the image would look like and retrieve results from the OCR 




# Wine-Quality-Prediction
## Task:
Build a Machine Learning Model to predict the quality of wine. We have been provided with a labelled dataset, so this will come under Supervised Learning.</br>
We are going to do the task as Binary Classification and we are going to use <b>Random Forest Classifier</b> to achieve the result. Random Forest CLassifier uses multiple Decision Tree models to predict the outcome.
## Dataset:
The dataset is being taken from Kaggle 'winequality-red'. The dataset contains 1599 records and 12 features. The features are:
fixed acidity</br>
volatile acidity</br>
citric acid</br>
residual sugar</br>
chlorides</br>
free sulfur dioxide</br>
total sulfur dioxide</br>
density</br>
pH</br>
sulphates</br>
alcohol</br>
quality</br>

Link: https://www.kaggle.com/datasets/brendan45774/wine-quality

## Steps Involved:
### Import Dependencies
Libraries needed for the task are:</br>
. numpy</br>
. pandas</br>
. matplotlib</br>
. seaborn</br>
. train_test_split from sklearn.model_selection</br>
. RandomForestClassifier from sklearn.ensemble</br>
. accuracy_score from sklearn.metrics</br>
### Data Collection
Use the read_csv function of pandas to import the dataset.</br>
shape, head and isnull() functions can be used to know our dataset.
### Data Analysis and Visualization
. We can use describe function to know about all the statistical measures of the features.</br>
' We have plotted some graphs to visually represent the relation between the feature and the label.</br>
. We have plotted heatmap to represent how each feature in the dataset is linked to the other features.</br>
### Data Preprocessing
We have separated the features from the label using the drop function.</br>
In the quality column which acts as a label here, we have 6 different values that are 3,4,5,6,7 and 8 all representing different levels of quality. As we are performing binary classification here, there is a need to convert these to 2 values. It can be represented as 0 and 1, where 1 includes values 7 and above which are of 'Good Quality' whereas 0 includes values from 6 and below which is of 'Bad Quality'. And finally, we had to store the quality in different variables.
### Split into train and test
In this, we had split the dataset into 4 parts x train, x test, y train and y test where y contains all the label data whereas x contains the features dataset.</br>
we have taken 20% of the data for training while the remaining 80% is kept for training purposes.
### Model Training
We have turned the dataset into a binary classification type and for this now we are going to use <b>Random Forest Classification.</b>
### Model Evaluation
we have performed the model evaluation on both the training and test data. The results are:</br>
Accuracy score for trained data:  1.0</br>
Accuracy score for test data:  0.925
### Building a Predictive System
For this, we have taken random data from the dataset and converted it into a numpy array and later reshaped it in order to feed it to the build model.</br></br></br>



Reference: Project 6. Wine Quality Prediction using Machine Learning with Python | Machine Learning Project, Siddhardhan, https://www.youtube.com/watch?v=CBxJuwrGrc4&list=PLfFghEzKVmjvuSA67LszN1dZ-Dd_pkus6&index=7


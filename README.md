# Bank Marketing Campaign
Customers of a Portugueuse Banking Institutuion were contacted mainly by phone, and other means more than once if required to access if they would subscribe to a fixed term deposit. 

### OBJECTIVE
- The main purpose of this project was to train a machine learning model based on the bank marketing data from a Portugueuse banking institution to determine if a customer\client will subscribe to a product(fixed term deposit).
- The minor aim of this project is to try feature selction ad feature engineering using featurewiz, a python library.


### PROCESS
- After checking for null values and unique values, I wet straight away to implementing feature engineering using featurewiz. 
-The data is mostly categorical so for it be more efficient and effective, I did encoding using the featurewiz once again, by setting the parameter, 'categorical_encoders=OneHotEncoding' and 'feature_engg='groupby' to group all categorical variables and encoding them and to create other features from them.
- Fourteen important features were selected and put into a dataframe, some from the original data and others generated during the process.
- The next thing was dropping all null values from the new dataframesplitting the data into two parts, train and test data.
- In order to find the classifier that would give the highest accuracy_score based on the features selected, I grouped four different classifiers and trained all together. The classifiers selected were [KNeighborClassifier, GradientBoosting, DecisionTree, RandomForest].
- Using the metrics; accuracy_score and mean absolute value, I finally chose GradientBoosting Classifier because it had the highest accuracy score of 91% and the least MAE of 0.08.


### NEXT
- Hyperparameter tuning using Gridsearchcv on the GradientBoostingClassifier model to see if the accuracy score would shoot up further.
- Then finally, this model could be used to predict if a client will agree to subscription given.


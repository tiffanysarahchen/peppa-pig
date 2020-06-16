# peppa-pig
Random Forest Classifier

Input data used for training contains raw accelerometer data collected using the 
Beiwe research platform (read more at https://github.com/onnela-lab/beiwe-backend )

Goal: Classify different physical activities using x, y, and z linear acceleration
measurements by training a random forest classifier model

random_forest_classifier:
File contains the code that runs a machine learning random forest classifier model
on data collected on an accelerometer. Input data includes linear acceleration on 
the x, y, and z axis. The code fits the model using various statistics, 
machine-learning, and number theory calculations.

data_visualization_code:
File contains the code that shows how visualization graphs were created to model
and see the relationship and fit of each independent variable that went into the 
model.

train_time_series:
CSV file that contains all the time indicators alongside each measurement of 
linear acceleration upon x, y, and z axis needed to fit the training set
Data has the following format: timestamp, UTC time, accuracy, x, y, z

train_labels.csv:
CSV file that contains all the time indicators wanted for each activity label
prediction. File also contains all the label indicators for the training set that
corresponds to train_time_series. Labels are only provided for every 10th 
observation in train_time_series

test_time_series.csv:
CSV file that contains all the time indicators alongside each measurement of 
linear acceleration upon x, y, and z axis needed to fit model to make predictions
Data has the following format: timestamp, UTC time, accuracy, x, y, z

test_labels.csv:
CSV file that contains all the time indicators wanted for each activity label
prediction. Label indicators correspond to every tenth observation in 
test_time_series

test_predictions.csv:
CSV file that contains all the output activity labels predicted by the model

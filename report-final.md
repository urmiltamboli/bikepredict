# Report: Predict Bike Sharing Demand with AutoGluon Solution
Urmil Tamboli

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
In order to submit the prediction, it was important to remove any predictions less than 0 and replace them by 0

### What was the top ranked model that performed?
WeightedEnsemble_L3 was ranked top for for all the three iterations

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
Exploratory analysis was done by plotting a histogram of all the feartures to see how the features are doing compared to the count; the datetime feature was broken down into year,month and day to provide extra features which could be used to get a better prediction

### How much better did your model preform after adding additional features and why do you think that is?
The model did not perform better by extra features into the dataset  

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
The model did perform good upon adding the hyperparameter compared to the second model but for the first model, the score dropped from when the hyperparameter were not being used, there could be a various reasons behind this results ie data sentivity , overfitting, not know proper hyperparamter values to add in

### If you were given more time with this dataset, where do you think you would spend more time?
If gives more time on this dataset, i would spend little more time on adding any other extra features and gain deeper understanding on hyperparameters which could make it easy for which hyperparameter to use and also try some other models other than Autogluon to see how they perform independently 

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
https://github.com/urmiltamboli/bikepredict/blob/e03f624f987b7d4b88af806bfc3470c52ed3b238/summ_table.png


### Create a line plot showing the top model score for the three (or more) training runs during the project.
https://github.com/urmiltamboli/bikepredict/blob/c525f57119447e8c6a0af72f4426f2a75e127a84/model_score.png


### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.
https://github.com/urmiltamboli/bikepredict/blob/c525f57119447e8c6a0af72f4426f2a75e127a84/kaggle_score.png


## Summary
The main goal of this project was to predict the bike sharing demand. Starting with installing all the required libraries and using the Kaggle API and downloading the dataset from Kaggle which already has been split between train and test datasets. Three iterations of model was run on this dataset using the AutoGluon algorithm. the first model was run without making any changes to be considered as a baseline which gave a score of 1.79, further new features were added which dropped the performance of the model; the last iteration on the model was done to tune the hyperparaters to see if the model would perform any better than the previous iteration. To our surprise, it didn't perform well compared to second model while it performaned better than second model and the score dropped to 1.31. If the model was to selected to go ahead, it would be from the first iteration. 

# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Nguyen Phung Hung

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: I realized that all the value in prediction always be greater or equal than zero. I need to chanege all value less than zero to equal to zero to submit my result

### What was the top ranked model that performed?
TODO: the top ranked model that performed was WeightedEnsembleModel

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
when conduct explored and analysis data, we can see the data about datetime column has an partitions all. So to do this column make a sense with data, i devied the column to year, month day, hour and so that the data can be make more sense

### How much better did your model preform after adding additional features and why do you think that is?
when adding more feature. we can see the score had be change from 0.67724 to 1.79605. I think the column datetime affect to the result of the trainning model

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
when we conduct to training several times. I think we can see the result after each training time and tunning all hyper parameters on some model like KNN or GBM. The result was better than previous training

### If you were given more time with this dataset, where do you think you would spend more time?
If i have more time with the dataset. i think i will focus about distribution of data. I will see the distribution on all column and change the distribution to normal distribution on all column

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|eval_metric=root_mean_squared_error	|auto_stack=False	|presets=[best_quality]	|1.79605|
|add_features|eval_metric=root_mean_squared_error	|auto_stack=False	|presets=[best_quality]	|0.67724|
|hpo|eval_metric=root_mean_squared_error	|auto_stack=False	|presets=[best_quality]	|0.45711|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png]

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png]

## Summary
By the project Predict Bike Sharing. I have some exprerience about using Sagemaker and Autogluon to processing, visualliztion data and traning model. 

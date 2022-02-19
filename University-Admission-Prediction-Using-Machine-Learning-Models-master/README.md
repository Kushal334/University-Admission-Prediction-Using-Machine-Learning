# University Admission Prediction Using Machine Learning Models

In this repository, I have implemented various machine learning models that predict whether the probability of a student getting accepted into a University offering a Masters degree. Upon noting the validation accuracies on each of the model, I have selected the best of all on them and shown how the key performance indicators(KPIs) vary in their values.
<br>

 
# Data

The dataset contains several parameters which are considered important during the application for Masters Programs.
The parameters included are :<br>

1) GRE Scores ( out of 340 )<br>
2) TOEFL Scores ( out of 120 )<br>
3) University Rating ( out of 5 )<br>
4) Statement of Purpose and Letter of Recommendation Strength ( out of 5 )<br>
5) Undergraduate GPA ( out of 10 )<br>
6) Research Experience ( either 0 or 1 )<br>
7) Chance of Admit ( ranging from 0 to 1 )<br>

# Citation

Mohan S Acharya, Asfia Armaan, Aneeta S Antony : A Comparison of Regression Models for Prediction of Graduate Admissions, IEEE International Conference on Computational Intelligence in Data Science 2019

# Model
<br>
For this dataset, we tried the following four models with their accuracies listed as below <br>

|   Model                |Validation Accuracy|
|------------------------|-------------------|
|Linear Regression     |   0.822831       |
|Artificial Neural Networks(5-layers)       |   0.805562       |
|Decision Tree    |   0.460020       |
|Random Forest           |   0.797299       |
<br>
As we can see, the best model is our Multiple Linear Regression model with a validation accuracy of 0.822831
<br>

# Insights
<br>

1) The mean for the GRE scores is 316<br>
2) Mean for TOEFL score is 107<br>
3) Standard deviation for the GRE score is 11, which suggests that about 68% of the students scored between 305 and 327<br>
4) Average University Ranking is 3<br>
5) There is a very high correlation between GRE and TOEFL scores. A student who scores higher on GRE tends to score higher on their TOEFL exam<br>
6) The chance of admission acceptance increases as GPA, SOP and University Ranking improve/increase<br>
7) Students who have research experience in the past, tend to have a higher chance of getting into a University with a ranking of 3<br>
<br>

![Analysis_Chart](https://github.com/Aishwarya4823/University-Admission-Prediction-Using-Machine-Learning-Models/blob/master/Images/Analysis.JPG)

# Key Performance Indicators(KPIs)
<br>
In the following text, I have explained what role each KPI plays and what the value that we have got suggests about our best model(Multi-Linear Regression)

## Mean Absolute Error(MAE)
<br>
We achieve a MAE of 0.0383 on the multiple linear regression model. Being a measure of the avg magnitude of error, as our MAE is very close to zero, we can say 
that our predictions are very close to the right predictions.
<br>

## Mean Square Error(MSE)
<br>
MSE, in this case, is 0.00268, which is a value close enough to 0. This tells us that there are very few outliers in the data since if there would have been a higher
number of outliers, the MSE value would have been higher.
<br>

## Root Mean Square Error(RMSE)
<br>
We can see that the RMSE value is 0.052. This tells us that the standard deviation of the residuals is a lower value.
<br>

## R^2 (Coefficient of Determination)
<br>
R-squared value is 0.82 which means that 82% of the variance in our dataset can be explained by the regression model.
<br>

## Adjusted R-squared value
<br>
We can see that the adjusted R-squared value is 0.80432. We can see that the value of adjusted R-squared is high which suggests that the predictors used in the model
are all useful. If there are any such predictors that do not play a significant role in predicting the outcome, Adjusted R-square value decreases as it penalises such predictor factors.






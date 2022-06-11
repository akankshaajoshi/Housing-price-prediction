# Housing-price-prediction
A simple machine learning model which predicts the prices of houses in King County, USA with an R2 Metric of 0.81. 

Dataset for this project is picked from Kaggle. It includes data of the houses sold between May 2014 and May 2015.
Dataset: https://www.kaggle.com/code/mayanksrivastava/predict-housing-prices-simple-linear-regression/data
Download using the API Call: kaggle kernels output mayanksrivastava/predict-housing-prices-simple-linear-regression -p /path/to/dest

Prediction model for housing prices can be viewed as a regression model as it deals with continuous data required for predictions.
Methodologies and approaches applied in this project are:

1.Data wrangling: Unreleated features(with very low correlation coefficients) were dropped and features with low feature importances were removed to simplify the model. Data with duplicated indices were dropped to avoid any complications.
 
2.EDA (Exploratory data analysis): Infographics were created using PyPlot and Seaborn to understand the relationship among data variables. Heatmaps describing the correlation between variables, histplots of price ranges, data descriptions and value counts for class intervals provide information regarding the data. 

3.Prediction model: Regression models such as Linear Regression, Lasso regression and Ridge regression were first evaluated to fit on the data set. However, due to their unsatisfactory metric evaluation, polynomial fit for ridge regression was tested.

4.Cross validation: Cross validation is done on the finally scaled and polynomial fitted feature data and label values.

An overall R2 Metric for the test data came out to be 81.5% for the test set and that for 4-fold validation test is given in the .ipynb file.

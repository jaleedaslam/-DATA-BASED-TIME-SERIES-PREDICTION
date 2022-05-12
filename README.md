# -DATA-BASED-TIME-SERIES-PREDICTION

# Goal

The goal is to use python software on a dataset and create a data-based time-series prediction model
that provided statistical forecast for confirmed cases of COVID-19 all over the world.

# Description of data
The dataset used from a Kaggle dataset that was retrieved by the Centre for Systems Science
and Engineering at Johns Hopkins University. It contained 8 features columns including deaths,
recovered and confirmed cases of COVID-19 and 75 no. of observations from Jan to mid of April.
10.3 Description of the model implementation and forecasting

# Model selection
After reviewing different papers and python software, related to data-based time-series prediction I
decided to apply Prophet which an open source library published by Facebook that provides the
ability to make time series predictions with good accuracy using simple intuitive parameters.

# Model implementation and forecasting
From dataset, no. of observation of the confirmed cases fit to the Prophet model with additive
seasonality and changepoint scale of 0.15 which is a key factor in forecasting accuracy and then
build a dataframe and on which fit daily predictions for the next 30 days. As in fig. red doted lines
shows changepoints where model detect sudden changes in the trend during model training. Black
dot shows the actual data points and confirmed cases predicted by the blue lines with upper and
lower limit. The plot shows a rapid increase in no.of cases from starting April and follow upward
trend.

#  Model evaluation
Model evaluation done by the using Prophet’s cross validation procedure which gives various
prediction performance metrics. I took and plotted MAPE for my model evaluation which is easier
to understand.

# Python Libs
- NumPy
- Pandas
- Scikit learn
- Matplotlib
- Seaborn
- Prophet 

# Prerequisite
- Python >= v3.8
- Jupyter Notebook
- knowledge of Time Series Data


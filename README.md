# Final Degree Project (TFG) Repository

This repository contains all the files and source code used in my Final Degree Project (TFG). Below is a detailed description of each folder and file present in the repository:

## Folders

### 1. DataSet
Contains the original datasets used in the study. These data served as the basis for the analyses and prediction models conducted. This folder is further divided into subfolders corresponding to each company. Each of these folders includes .csv files related to daily stock prices and market capitalization, as well as quarterly data on balance sheets, ratios, earnings, and cash flow.

### 2. Stationarity
This folder contains the results of the stationarity analysis. Crucial for data preprocessing in time series modeling, this analysis ensures that the data meet the necessary assumptions for prediction models. Here, you'll find the .xlsx files where the results of the ADF test, among others, are stored, both before and after conversion to stationarity. Also included are the .xlsx and .csv files of the stationary datasets.

### 3. TFG Figures
Here are all the figures and graphs generated during the study. These graphics illustrate the key results and findings obtained during the analysis. Additional graphs not included in the TFG report can be found in the Jupyter notebooks.

### 4. Hypertunning
This folder contains the results of hyperparameter tuning for the LSTM network. It includes preliminary results for four of the six companies studied. For the other two, we decided to keep only the best combination instead of generating .xlsx files, for computational efficiency. These results were slightly modified in search of greater efficiency.

### 5. Merged_Data
This folder contains the original data that has been processed and combined for analysis. These are the data prior to those obtained in the stationarity folder.

## Jupyter Notebook Files

### 1. Data_Processing.ipynb
This Jupyter notebook contains the code for data processing. It ranges from importing files from Merged_Data to creating financial indicators and the target variable. It also shows the results of the stationarity study and outlier analysis. It concludes with the creation of lags and a series of useful visualizations that were included in the TFG report.

### 2. Models_Archivo_Final.ipynb
This Jupyter notebook contains the code for building and evaluating machine learning models. It includes everything from applying PCA and Lasso to our input sets (applying a grid search of hyperparameters to optimize them), auxiliary functions for splitting the set into training and test, for scaling and dimensionality reduction, transforming percentage increase to nominal value, and creating a dataframe (result_df) with the prediction and the actual nominal values, as well as the implementation of the LSTM network, XGboost, Random Forest, and Linear Regression, along with the parameter optimization of the first two.

## Other Files
### 1. Resultados_Lasso_ACP.txt
This text file shows the execution when applying the code for dimensionality reduction. It displays the terminal output related to the variables chosen by Lasso with and without lags, and the same for PCA.
### 2. FernándezdelAmoPablo_TFG.pdf
TFG report, which presents both the theoretical framework of the work's development and the results obtained.

If you have any questions about this repository or the work in general, please do not hesitate to contact me.


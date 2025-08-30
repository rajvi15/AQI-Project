# AQI-Project
AQI Prediction Project
This Project Predicts the Concentration of Pollutants.
Here's a complete data preprocessing pipeline designed to clean and prepare an air quality dataset for a machine learning model that will predict PM2.5 concentrations.

The process involves these key stages:
1). Data Cleaning: It begins by loading the data and identifying missing values. Crucially, it removes any records where the PM2.5 value itself is missing and then fills (imputes) gaps in other pollutant columns using their median values.
2). Feature Engineering: The script enhances the dataset by converting the Date column into a usable format and extracting new features like year, month, and day. It also transforms the categorical City column into a numerical format using one-hot encoding and removes columns like AQI to prevent data leakage.
3). Model Preparation: Finally, it separates the data into features (X) and the target (y). The data is then split into training and testing sets and scaled using StandardScaler to ensure all features have a similar range, making them ready to be fed into a machine learning model.

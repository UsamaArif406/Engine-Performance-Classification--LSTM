#Project Overview
This project involves preprocessing a dataset with various engine-related features to train a Long Short-Term Memory (LSTM) model for classifying the operational status of the engine. The primary goal is to predict the status of the engine based on historical data.

# Dataset
The dataset contains the following columns:

TimeStamp: Date and time of the observation
Ambient Temperature
Distance Travelled
Engine Coolant Temperature
Engine Fuel Rate
Engine Intake Manifold Pressure
Engine Intake Manifold Temperature
Engine Oil Pressure
Engine Oil Temperature
Engine RPM
Idle
Machine Running Hours
Machine Speed
Operational
Transmission Hours
Transmission Oil Pressure
Transmission Oil Temperature
status: The target variable indicating the operational status of the engine

# Usage
## Data Preprocessing
The data preprocessing script sorts the dataset by TimeStamp, standardizes the features, and creates sequences for the LSTM model. The steps are:

Sort the DataFrame by TimeStamp.
Drop the TimeStamp column as it is not needed as a feature for the model.
Encode the status labels.
Standardize the features.
Create sequences of a specified length.

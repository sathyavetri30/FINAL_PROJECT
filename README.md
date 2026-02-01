Advanced Time Series Forecasting Using Transformer and Attention
Project Description

This project focuses on multivariate time series forecasting using a Transformer-based deep learning model with self-attention. The objective is to predict Global Active Power consumption from historical power usage data indexed only by a time column. The Transformer model is evaluated against a traditional XGBoost baseline to demonstrate performance improvements using attention mechanisms.

Dataset

Multivariate time series dataset

Contains a single time column used as the datetime index

Multiple power-related numerical features

Missing values handled using time-based interpolation

Features Used

Global Active Power (target)

Global Reactive Power

Voltage

Global Intensity

Sub Metering 1

Sub Metering 2

Sub Metering 3

Methodology

Convert time column to datetime index

Normalize features using StandardScaler

Create sliding window sequences

Train Transformer model with self-attention

Train XGBoost model with lag features

Compare models using standard evaluation metrics

Models Implemented

Transformer Encoder (PyTorch)

XGBoost Regressor (Baseline)

Evaluation Metrics

RMSE (Root Mean Squared Error)

MASE (Mean Absolute Scaled Error)

sMAPE (Symmetric Mean Absolute Percentage Error)

Tools & Technologies

Python

Pandas, NumPy

PyTorch

Scikit-learn

XGBoost

Output

Trained Transformer model saved as .pth file

Performance comparison between deep learning and baseline models

Conclusion

The Transformer-based model outperforms the baseline approach by effectively capturing long-term temporal dependencies using attention mechanisms, making it suitable for real-world power consumption forecasting tasks.

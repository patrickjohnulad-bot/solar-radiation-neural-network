# Solar Radiation Prediction Using Neural Networks

## Problem
Predict solar radiation (W/m²) 5 minutes to 2 hours in advance using historical weather data.

## Dataset
- 32,686 samples at 5-minute intervals
- Features: temperature, humidity, pressure, wind, lagged radiation values
- Source: NASA solar radiation measurements

## Model Architecture
- 4 hidden layers: 128 → 64 → 32 → 16 neurons
- Batch Normalization + Dropout (0.2) + ReLU activation
- Framework: PyTorch

## Results
- R² Score: 0.9366
- MAE: 31.62 W/m²
- RMSE: 78.46 W/m²

## Key Finding
The model explains 93.7% of solar radiation variance, proving that deep learning can effectively forecast solar energy output.

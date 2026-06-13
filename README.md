# Solar Radiation Prediction Using Neural Networks

## Problem Statement

Solar energy is intermittent. When clouds block the sun, power output can drop 50-80% within minutes. Grid operators cannot react fast enough, forcing them to keep expensive backup power plants running or risk blackouts.

I propose to use a 4-layer neural network (128→64→32→16→1) to predict solar radiation 5 minutes to 2 hours in advance in order to help grid operators prepare for power fluctuations before they happen.

With accurate predictions, grid operators can reduce backup power costs, prevent blackouts, and maximize solar energy utilization.


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

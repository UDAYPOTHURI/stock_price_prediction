# Apple Stock Price Prediction

This repository contains a project to predict Apple stock prices using an LSTM (Long Short-Term Memory) neural network built with PyTorch. The dataset used consists of historical stock prices of Apple Inc. The project involves preprocessing the data, creating sequences, building an LSTM model, and training it to predict stock prices.

## Project Structure

- `StockPricePrediction.ipynb`: Jupyter notebook containing the entire workflow from data loading to model training and evaluation.
- `AAPL_2006-01-01_to_2018-01-01.csv`: Dataset used for training and testing the model.
- `README.md`: Documentation for the project.

## Dataset

The dataset `AAPL_2006-01-01_to_2018-01-01.csv` contains the following columns:

- `Date`: Date of the stock price
- `Open`: Opening price of the stock
- `High`: Highest price of the stock during the day
- `Low`: Lowest price of the stock during the day
- `Close`: Closing price of the stock
- `Volume`: Number of shares traded
- `Name`: Name of the stock

## Preprocessing

The preprocessing steps include:

1. Plotting the `Close` prices over time.
2. Checking for and handling any missing values.
3. Normalizing the `Close` prices using `MinMaxScaler`.
4. Creating sequences and labels from the normalized data.

## Model

The LSTM model is built using PyTorch and has the following structure:

- Input layer with 1 feature
- LSTM layer with 50 hidden units and 2 hidden layers
- Fully connected layer with 1 output unit for predicting the stock price

## Training

The training process involves:

1. Splitting the data into training and testing sets.
2. Training the model for 100 epochs.
3. Recording the training and testing losses for each epoch.

## Evaluation

The model's performance is evaluated by plotting the training and testing losses over the epochs.

## Dependencies

- pandas
- numpy
- scikit-learn
- torch
- torchinfo
- matplotlib

## Results

The training and testing losses are plotted to show the model's performance over the epochs. The model can also be used to predict the stock price of Apple given historical data.

## Conclusion

This project demonstrates a basic approach to predicting stock prices using an LSTM neural network in PyTorch. Further improvements can be made by tuning the model architecture, experimenting with different loss functions and optimizers, and using more advanced preprocessing techniques.

# Time-Series Transformer Forecasting

A time-series forecasting project exploring **PatchTST**, a Transformer-based architecture designed for long-term multivariate time-series forecasting.

## Objective

The project investigates how patch-based tokenization and channel-independent modeling can improve long-term forecasting performance.

## Approach

The experiments use PatchTST with different:

- Look-back windows
- Patch lengths
- Prediction horizons

PatchTST divides a time series into patches and processes them using a Transformer encoder for forecasting future values.

```text
Time Series
     ↓
Patching
     ↓
Patch Embeddings
     ↓
Transformer Encoder
     ↓
Forecast
```

## Models

The project compares:

- **PatchTST**
- **Linear baseline**
- **LSTM baseline**

## Evaluation

Models are evaluated using:

- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**

Experiments analyze how **context length, patch configuration, and forecasting horizon** affect model performance.

## Tech Stack

**Python | PyTorch | Transformers | Pandas | NumPy | Matplotlib**

## Project Structure

```text
Time-Series-Transformer-Forecasting/
├── data/
├── models/
├── experiments/
├── notebooks/
├── results/
└── README.md
```


## Future Work

- Experiment with additional time-series datasets
- Perform hyperparameter optimization
- Compare against additional Transformer architectures
- Investigate longer forecasting horizons

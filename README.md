# ARIMA Time Series Analysis

A hands-on Jupyter notebook exploring **Autoregressive (AR)** and **Moving Average (MA)** models for time series analysis using Python.

## Overview

This notebook walks through the simulation, visualization, and estimation of ARMA-family models, covering both synthetic data and real-world CSV datasets.

## Topics Covered

- **AR(1) & AR(2) Models** — Manual simulation using recursive formulas and fitting with `statsmodels` ARIMA
- **MA(1) & MA(2) Models** — Construction from white noise errors and parameter estimation
- **`arma_generate_sample`** — Generating ARMA processes using `statsmodels.tsa.arima_process`
- **ACF & PACF Plots** — Autocorrelation and Partial Autocorrelation analysis for model identification
- **Real Data Fitting** — Loading external CSV time series (`auto_1`, `auto_2`) and selecting appropriate AR/MA orders based on ACF/PACF patterns

## Dependencies
```bash
pip install numpy pandas matplotlib seaborn statsmodels
```

## Usage

1. Clone the repo and place your `auto_1.csv` and `auto_2.csv` files in the working directory.
2. (Optional) Add a `colorsetup.py` with custom `colors` and `palette` variables for styling.
3. Run the notebook cell by cell to simulate, visualize, and fit ARMA models.

## Key Concepts

| Model | AR params | MA params |
|-------|-----------|-----------|
| AR(1) | φ₁ = 0.7  | —         |
| AR(2) | φ₁ = 0.3, φ₂ = 0.3 | — |
| MA(1) | —         | θ₁ = 0.4  |
| MA(2) | —         | θ₁ = 0.4, θ₂ = −0.4 |

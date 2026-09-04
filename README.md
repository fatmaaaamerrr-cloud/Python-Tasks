# Time Series Analysis: Monthly Beer Production in Australia (1956–1995)

## Project Overview
Complete time series analysis of Australian monthly beer production data.  
Includes exploratory analysis, smoothing, decomposition, residual diagnostics, ARIMA/SARIMA modeling, forecasting, and model evaluation.

## Dataset
- **Source**: Monthly beer production in Australia (1956–1995)
- **File**: `Dataset 4_ monthly-beer-production-in-austr.csv`
- **Observations**: 476 months
- **Unit**: Megalitres

## What I Did
1. Data cleaning & preparation
2. Exploratory analysis (trend + strong seasonality)
3. Stationarity tests (ADF & KPSS)
4. Seasonal decomposition (additive vs multiplicative)
5. SARIMA modeling with grid search
6. Residual diagnostics (Ljung-Box, ACF/PACF, Q-Q plot)
7. Out-of-sample forecasting (24-month hold-out)
8. Model comparison (diagnostics-selected vs best-AIC)

## Key Results
- Strong annual seasonality + non-linear trend
- Final model: SARIMA on log-transformed series
- MAPE ≈ 6% on 24-month hold-out
- Residuals consistent with white noise

## How to Run
```bash
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn
jupyter notebook "TSA_Beer_Production_Final_Project (2).ipynb"

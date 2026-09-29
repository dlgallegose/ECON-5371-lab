# ECON-5371-lab

Labs for ECON-5371 (Econometrics/Time Series).

## Labs

- [Lab_1](Lab_1) — Non-Stationary Models, Seasonality (Week 5)
- [Lab_2](Lab_2) — Time Series Forecasting with ARIMA

## Lab 1 — Non-Stationary Models, Seasonality (Week 5)

Applies unit root testing (ADF, KPSS), ARIMA identification, SARIMA estimation, and residual diagnostics to a synthetic quarterly series with a stochastic trend and seasonal pattern.

- [lab_1.py](Lab_1/lab_1.py) — lab script
- [gdp_synthetic.csv](Lab_1/gdp_synthetic.csv) — synthetic quarterly business activity index data
- [Lab_1_Prep.pdf](Lab_1/Lab_1_Prep.pdf) — prep materials

Requires a dedicated Python environment (`conda create -n econ5371 python=3.11`) with `pandas`, `statsmodels`, and `pmdarima` — see the setup instructions at the top of `lab_1.py`.

## Lab 2 — Time Series Forecasting with ARIMA

Builds and evaluates ARIMA models on a synthetic monthly "Widget Sales Index" (2018–2025, trend + seasonality + autocorrelated noise): stationarity testing and differencing, ACF/PACF order identification, fitting candidate models, residual checks, out-of-sample forecasts, AIC/BIC comparison, and forecast evaluation.

- [lab_2.py](Lab_2/lab_2.py) — lab script
- [widget_sales.csv](Lab_2/widget_sales.csv) — synthetic monthly widget sales index data
- [generate_synthetic_data.py](Lab_2/generate_synthetic_data.py) — script that generates `widget_sales.csv`
- [requirements.txt](Lab_2/requirements.txt) — required packages

Uses the same Python environment as Lab 1 (`conda create -n econ5371 python=3.11`). From the `Lab_2` folder, install the packages with:

```
conda activate econ5371
pip install -r requirements.txt
```

Before running, set `LAB_FOLDER` near the top of `lab_2.py` to the `Lab_2` folder's path on your computer. Then run it cell by cell (`# %%` markers) or top to bottom with `python lab_2.py`.

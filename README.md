# 💨 Offshore Wind Profile Forecasting

Machine-learning model for **NOAA offshore wind profiles (USA)** — predicting wind characteristics from atmospheric reanalysis data using Random Forest regression.

## Overview
`offshore-wind-profiles.ipynb` builds a regression model over gridded meteorological data (ERA5 / NBS reanalysis), covering the full workflow:

- **Ingesting netCDF** climate data (`xarray` / `netCDF4`) and converting to tabular features
- **Feature engineering** from atmospheric variables (wind components, pressure levels, time)
- **Random Forest regression** to predict wind profiles
- **Evaluation** — RMSE / R², feature importance, error analysis by region/time

## Why it matters
Accurate offshore wind profiling supports renewable-energy siting and turbine yield estimation — a real-world regression problem on large, multi-dimensional geophysical data.

## Run it
```bash
pip install -r requirements.txt
jupyter notebook offshore-wind-profiles.ipynb
```

> The netCDF reanalysis files (e.g. ERA5 `*.nc`) are large and **not committed**.
> Download from the [Copernicus Climate Data Store](https://cds.climate.copernicus.eu/) (ERA5)
> or [NOAA](https://www.noaa.gov/) and point the notebook at your local path.

## Author
**Vamshi Krishna Damidi** — Data & AI Engineer
🌐 [Portfolio](https://vkdvamshi.github.io) · 💼 [LinkedIn](https://www.linkedin.com/in/vamshi-krishna-damidi-b6434512/) · 🐙 [GitHub](https://github.com/vkdvamshi)

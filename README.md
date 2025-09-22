# Smart Inventory & Demand Forecasting for Multi-Store Retail

## Overview  
This project was developed as part of the ADS-505 course final team project. The goal is to forecast daily product demand at the store–SKU level and translate forecasts into practical inventory decisions such as reorder points and safety stock. By doing so, the project addresses stockouts, overstocks, and helps quantify effects of price, promotions, holidays, and weather on demand.

## Objectives  
- Reduce stockouts and overstocks  
- Quantify drivers of demand (price, promotions, holidays, weather)  
- Deliver an executive-facing Tableau dashboard with KPIs and drill-downs

## Dataset  
We use a synthetic retail dataset (~73,000 rows; 2022–2023 daily granularity) containing:  
- Date, Store ID, Product ID, Category, Region  
- Inventory Level, Units Sold, Units Ordered, Demand Forecast, Price  
- Holiday, promotion, and weather indicators (if available)  

This dataset supports time-series forecasting and driver analysis across stores and categories.

## Methods  
- **Data Preparation:** Cleaning, feature engineering (calendar, promo, price), handling missing values  
- **Forecasting Models:** Seasonal Naïve, Prophet, tree-based models (LightGBM), exploratory LSTM  
- **Evaluation Metrics:** MAPE and MAE, with prediction intervals  
- **Business Translation:** Forecasts converted into reorder points and safety stock calculations  
- **Visualization:** Tableau dashboard for executives, including KPIs, filters, and drill-downs

## Repository Structure  
- `data/` – Raw and processed datasets (synthetic)  
- `notebooks/` – Jupyter notebooks for EDA, modeling, and evaluation  
- `scripts/` – Python scripts for cleaning, forecasting, and utilities  
- `dashboard/` – Tableau files and exports  
- `docs/` – Project documentation, including the business brief and final report  
- `README.md` – Project overview (this file)

## Results  
Models improve forecast accuracy over baselines and translate those gains into practical stocking guidance. The Tableau dashboard highlights stockout risks, overstock pockets, and allows merchandisers to drill into store or product levels for decision making.

## Team  
- Jami McMillen  
- Shivam Patel  
- Mark Henry Villanueva  

## License  
This project uses synthetic data and is intended for academic purposes only.

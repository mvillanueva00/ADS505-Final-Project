# Smart Inventory & Demand Forecasting for Multi-Store Retail

This project is a part of the ADS-505 course in the Applied Data Science Program at the University of San Diego.  

-- Project Status: Active  

---

## Installation  
Clone the repository and install required Python packages from `requirements.txt`.  
Run Jupyter notebooks in the `notebooks/` folder to reproduce data cleaning, feature engineering, and modeling.  
The Tableau dashboard file is included in the `dashboard/` folder for visualization.  

---

## Project Intro/Objective  
The main purpose of this project is to forecast daily product demand at the store–SKU level and translate forecasts into practical inventory decisions such as reorder points and safety stock. The goals are to reduce costly stockouts and overstocks, quantify drivers of demand like price and promotions, and deliver insights through an executive-facing Tableau dashboard. This will enable merchandisers and planners to make faster and more informed decisions.  

---

## Partner(s)/Contributor(s)  
- Jami McMillen  
- Shivam Patel  
- Mark Henry Villanueva  

---

## Methods Used  
- Predictive Modeling  
- Machine Learning  
- Time-Series Forecasting  
- Data Visualization  
- Data Manipulation  
- Feature Engineering  

---

## Technologies  
- Python  
- Google Colab  
- Tableau  
- GitHub  

---

## Project Description  
We use a synthetic retail dataset (~73,000 rows; 2022–2023 daily granularity) with fields such as Date, Store ID, Product ID, Category, Region, Inventory Level, Units Sold, Units Ordered, Demand Forecast, and Price. Holiday, promotion, and weather indicators are included where available.  

Our approach begins with data cleaning and feature engineering (calendar features, price and promotion flags, lags, and rolling statistics). Baseline models such as seasonal naïve and Prophet are used for initial forecasting. We then evaluate advanced methods including LightGBM and exploratory LSTM models. Models are assessed with MAPE and MAE metrics, and outputs are translated into inventory rules such as reorder points and safety stock.  

The final deliverable includes a Tableau dashboard with KPIs, trend visualizations, store and region heatmaps, and interactive drill-downs to identify stockout risks and overstock pockets.  

---

## License  
This project uses synthetic data and is intended for academic purposes only.  

---

## Acknowledgments  
We would like to thank the University of San Diego Applied Data Science program faculty for their guidance throughout the course.  

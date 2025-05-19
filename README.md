#  Toronto Airbnb Data Science Project

An end-to-end data science project analyzing short-term rental prices and activity in Toronto using R. This project combines geospatial mapping, time series analysis, and machine learning (XGBoost) to uncover insights into the Airbnb market and predict listing prices.

---

##  Project Highlights

* Cleaned and preprocessed raw Airbnb listing and review data
* Parsed spatial neighborhood boundaries using GeoJSON
* Conducted exploratory data analysis (EDA) on pricing and review behavior
* Built and evaluated XGBoost regression models (raw + log-transformed)
* Visualized geospatial price distribution using `leaflet`
* Analyzed feature importance and residuals for modeling insight
* Rendered all outputs into a self-contained HTML report with visualizations

---

##  Dataset Sources

1. **Airbnb Toronto Listings** (listings.csv)
2. **Airbnb Reviews** (reviews.csv)
3. **Toronto Short-Term Rental Program** (program\_summary.csv)
4. **City Registrations** (registrations.csv)
5. **Toronto Neighborhoods GeoJSON** (toronto\_neighbourhoods.geojson)

##  Tools and Technologies

* Language: `R`
* Notebook: `RMarkdown`
* Visualization: `ggplot2`, `leaflet`, `corrplot`, `GGally`
* Modeling: `xgboost`, `Matrix`
* Spatial Analysis: `sf`, `geojson`
* EDA: `dplyr`, `janitor`, `scales`, `lubridate`

---

## Key Visuals and Analysis

### Exploratory Data Analysis

* Distribution of price across listings (histogram)
* Review activity over time (time series)
* Review counts per listing and normalized engagement

### Geospatial Mapping

* Choropleth map of average price by neighborhood
* Map of average reviews per listing

### Correlation & Feature Analysis

* Correlation heatmap of numeric variables
* GGally matrix for paired numeric feature insights

###  Predictive Modeling (XGBoost)

* Model 1: Raw price prediction

  * RMSE: \~87.54
  * MAE: \~50.08
  * R²: 0.594
* Model 2: Log(price+1) prediction (back-transformed)

  * RMSE: \~88.54
  * MAE: \~47.73
  * R²: 0.585
* Feature Importance (top 20 visualized)
* Residual plot for error inspection

---

## Report Output

The full analysis is available in the HTML report with integrated plots and explanations:

 open `report.html` from the repository to view locally.

---

##

##  Author

**Trivikram Madala**
Graduate Certificate in Business Insights & Analytics
Humber College, Toronto

##  License

This project is for academic and portfolio purposes. Data used is publicly available via Open Data Toronto and InsideAirbnb.

##  Acknowledgements

* [City of Toronto Open Data Portal](https://open.toronto.ca/)
* [InsideAirbnb](http://insideairbnb.com/)
* [XGBoost Developers](https://xgboost.readthedocs.io/)

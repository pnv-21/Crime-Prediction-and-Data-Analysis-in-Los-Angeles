# LA Crime Prediction and Data Analysis

This project analyzes crime incidents in Los Angeles and predicts future monthly crime counts by area using machine learning. It also visualizes spatial and temporal crime patterns to support strategic planning and resource optimization.

## Objectives

- Identify trends and patterns in crime types, locations, and time
- Predict monthly crime volumes by area using historical data
- Present visual insights through maps and time series graphs

## Dataset

- Source: Los Angeles Open Data Portal
- Time Range: 2020 to 2023
- Key Fields: Date, Time, Area Name, Crime Code, Description, Latitude, Longitude

## Analysis Highlights

- Top five crime types identified with monthly and hourly breakdown
- Temporal analysis revealed crime spikes in summer months and weekdays
- Hourly categorization (Midnight, Morning, Afternoon, Evening) uncovered peak times
- K-Means clustering visualized geographical hotspots across neighborhoods
- Heatmaps and line plots highlighted long-term and seasonal trends

## Prediction

- Model: XGBoost Regressor
- Features: Area name, month, crime category, time-of-day grouping
- Target: Monthly crime count per area

**Evaluation Metrics:**
- Mean Absolute Error (MAE): ~22 crimes per area
- Root Mean Squared Error (RMSE): ~29 crimes per area

The model was validated on 2023 data and used to forecast monthly crime counts for 2024 across all LAPD divisions. Results were visualized as a pivot table and multi-line chart by area.

## Maps

- **Crime Density Map**: Used `folium.plugins.MarkerCluster` to visualize clusters of incidents by location  
- **Time-based Crime Distribution Map**: Layered markers by crime type and time category using color-coded `CircleMarker` groups

## Technologies Used

Python  
Pandas  
Folium  
Matplotlib  
Seaborn  
Scikit-learn  
XGBoost

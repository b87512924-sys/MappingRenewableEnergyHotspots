# MappingRenewableEnergyHotspots
ML-powered geospatial analysis for solar energy site selection in Rajasthan using satellite data
Student: Anushka Bansode
Mentor: Tanvi Anand
# Solar Energy Hotspot Prediction in Rajasthan, India

## Project Overview
This project identifies and predicts solar energy hotspots in Rajasthan, India using geospatial data and machine learning. Developed as part of the WiDS (Women in Data Science) initiative under the theme "ML meets sun and wind," this work demonstrates how machine learning can enhance renewable energy resource mapping.

## Methodology

###  Data Collection & Processing
The analysis leverages Google Earth Engine to extract multiple geospatial datasets for 2023:
- **Solar Data**: Global Horizontal Irradiance (GHI) from NASA POWER/MODIS
- **Terrain Data**: Elevation, slope, and aspect from USGS SRTMGL1_003
- **Land Cover**: NDVI, Land Cover classification, Bare Soil Index, and Albedo
- **Climate Data**: Temperature, cloud cover, wind speed, and precipitation

###  Study Area
Focuses on Western Rajasthan with 500 sample points for comprehensive spatial analysis. The region was selected for its high solar potential and relevance to India's solar energy goals.

###  Machine Learning Pipeline
Four regression models were implemented and compared:
- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **XGBoost Regressor** (Best performer: R² = 0.890, MAPE = 0.20%)

###  Key Results
1. **Top Predictors**: Elevation, land surface temperature, and cloud cover showed strongest correlation with GHI
2. **Hotspot Identification**: Western Rajasthan consistently showed 'Excellent' solar potential
3. **Validation**: Model predictions aligned well with known solar parks (Bhadla, Nokh, Fatehgarh)

## Technical Implementation

### Core Workflow
1. **Environment Setup**: Google Earth Engine authentication and library imports
2. **Data Extraction**: Multi-source geospatial data collection
3. **EDA & Visualization**: Comprehensive analysis and interactive mapping
4. **Model Training**: Regression model development and evaluation
5. **Hotspot Mapping**: Predictive modeling across Rajasthan grid

### Outputs Generated
- Interactive Folium maps for solar potential visualization
- Trained XGBoost model for GHI prediction
- Identified solar hotspots with top 10 locations
- Comprehensive performance metrics and analysis reports

## Impact & Applications
This project provides a scalable framework for:
- Solar farm site selection and planning
- Renewable energy resource assessment
- Integration of ML with geospatial analysis for environmental applications
- Supporting India's transition to clean energy

## Technologies Used
- **Python**: pandas, numpy, scikit-learn, xgboost
- **Geospatial**: Google Earth Engine, Folium
- **Visualization**: matplotlib, seaborn
- **Data Processing**: Joblib for model serialization


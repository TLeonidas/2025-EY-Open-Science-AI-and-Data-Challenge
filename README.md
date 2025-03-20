# Urban Heat Island (UHI) Prediction Model

## Overview
This open-source machine learning project is part of the **2025 EY Open Science AI & Data Challenge**. It aims to predict **Urban Heat Island (UHI) hotspots** at micro-scales (meters) across New York City using a combination of ground temperature data, satellite imagery, building footprints, and weather data.

## Objectives
- Develop an ML model to predict UHI index values across NYC.
- Improve upon the baseline model provided by EY.
- Ensure model interpretability to highlight key urban factors affecting UHI hotspots.
- Maintain an open-source approach for scalability to other cities.

## Dataset Sources
### Provided Datasets
- **Ground Temperature Data** (CAPA Strategies) – 11,229 data points collected on July 24, 2021.
- **Building Footprints** (Cornell University Geospatial Information Repository).
- **Sentinel-2 Optical Satellite Data** (Microsoft Planetary Computer) – NDVI, urban density.
- **Landsat Surface Temperature Data** (NASA, Microsoft Planetary Computer).
- **Local Weather Data** (New York State Mesonet) – Temperature, humidity, wind speed/direction, solar flux.

### Additional Considerations
- Open-source geospatial datasets for finer resolution analysis.
- Historical weather trends for temporal analysis.

## Approach
### **1. Data Preprocessing**
- Convert all datasets to a common geospatial coordinate system.
- **Feature Engineering**: Compute building density, proximity to green spaces/water bodies.
- Normalize data and split into train (70%) / validation (30%).

### **2. Model Development**
#### Baseline Model
- **Linear Regression** using Sentinel-2 features.

#### Advanced Models
- **Random Forest Regressor** (for feature importance analysis).
- **Gradient Boosting (XGBoost, LightGBM, CatBoost)**.
- **Neural Networks (MLP with Geospatial Features)**.
- **Graph Neural Networks (Optional, if modeling spatial relationships)**.

### **3. Model Evaluation**
- **Primary Metric**: R² Score (≥ 0.8 required for challenge).
- **Secondary Metrics**: MAE, RMSE.
- Feature importance analysis.

### **4. Deployment & Open-Source Contributions**
- **GitHub Repository** for full code & documentation.
- **Jupyter Notebook** with clear explanations and visualizations.
- **Step-by-step instructions** for data preprocessing and model training.

## Next Steps
1. Set up data preprocessing scripts.
2. Develop baseline model & evaluate performance.
3. Iterate with advanced models & optimize.
4. Analyze feature importance & interpretability.
5. Document findings & prepare open-source release.

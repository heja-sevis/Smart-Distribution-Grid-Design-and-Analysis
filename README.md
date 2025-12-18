# ⚡Smart Distribution Grid Design and Analysis

An intelligent decision-support system for electrical distribution network planning, voltage drop analysis, load forecasting, and anomaly detection.
This application leverages Streamlit, Machine Learning, and Geospatial Analysis to optimize grid infrastructure and monitor performance.

**🔗 Live:** [Smart Distribution Grid Design and Analysis View the Dashboard on Streamlit](https://smart-distribution-grid-design-and-analysis.streamlit.app)

---

## 🚀 Project Overview and Features

The application consists of four core modules:
* **1.Demand Input & Route Planning :**
    * Interactive map-based selection of new demand points.
    * Automated route generation between the demand point and the nearest transformers.
    * Smart "snapping" to existing poles within a defined radius.
    * Comparison of candidate transformers based on capacity and voltage drop.
* **2.Voltage Drop Analysis (Formula vs. ML) :**
    * Calculates voltage drop using both the standard engineering formula ($k \cdot L \cdot N$) and a trained Machine Learning model (LightGBM/RandomForest).
    * Visual comparison of ML predictions against theoretical values for selected transformers
* **3. Forecasting:**
    * Time-series prediction of grid load using the Prophet model.
    * Supports daily mean/total aggregations.
    * Includes confidence intervals and performance metrics (RMSE, MAE, MAPE).
* **4. Fault & Anomaly Detection:**
    * Unsupervised learning using Isolation Forest to detect electrical anomalies.
    * Visualizes current-voltage deviations to identify potential grid faults. 

## 🛠 Technical Stack

| Category | Tools |
| :--- | :--- |
| **Framework** | Streamlit |
| **Geospatial** | Folium, Geopy, Shapely, PyProj |
| **Machine Learning** | Prophet, Scikit-Learn, LightGBM |
| **Data Handling** | Pandas, NumPy, OpenPyXL |
| **Visualization** | Plotly Express, Matplotlib |

---

# Air Pollution Forecasting using ML and DL Models

![License](https://img.shields.io/badge/license-CC%20BY--NC--ND%204.0-blue)
![Python](https://img.shields.io/badge/python-3.8+-blue)
![Status](https://img.shields.io/badge/status-Research%20Project-brightgreen)

## 📘 Project Overview

This repository contains the complete implementation and analysis of a research study focused on forecasting PM2.5 and PM10 concentrations using both traditional machine learning models and deep learning (LSTM) networks. The study evaluates the effectiveness of various models in predicting air quality for five major cities in Maharashtra, India, using real-time pollution and meteorological data from 2019 to 2023.

## 🧠 Models Implemented

- 📈 **Decision Tree**
- 🌲 **Random Forest**
- ⚡ **XGBoost**
- 🧠 **LSTM (Long Short-Term Memory Network)**

## 🗂 Dataset

- Source: [Central Pollution Control Board (CPCB), India](https://airquality.cpcb.gov.in)
- Duration: January 2019 – March 2023
- Locations: Mumbai, Pune, Aurangabad, Nasik, Thane
- Key features:
  - PM2.5, PM10
  - NO, NO₂, CO, SO₂, O₃, Benzene, Toluene
  - Temperature, Wind Speed, Wind Direction, Humidity

## ⚙️ Methodology

1. **Data Collection** from CPCB air monitoring stations
2. **Data Pre-processing**:
   - Handling missing values
   - Outlier removal using Z-score
   - Log-transformations for skewed features
   - Feature scaling (Min-Max)
   - Multicollinearity analysis (VIF)
3. **Model Training and Tuning**:
   - GridSearchCV and RandomizedSearchCV for hyperparameter optimization
   - Evaluation metrics: R² Score, RMSE
4. **Deep Learning (LSTM)**:
   - 3 LSTM layers + Dense layer
   - Dropout for regularization
   - Trained with 100 epochs, batch size = 1

## 📊 Results

| Model           | Best R² Score | Best RMSE  |
|----------------|---------------|------------|
| Decision Tree  | 0.78          | ~9-14      |
| Random Forest  | 0.87          | ~8-12      |
| XGBoost        | 0.91          | ~7-10      |
| **LSTM**        | **0.9999**    | **0.15**   |

> 🥇 **LSTM outperformed all ML models with near-perfect accuracy and the lowest error.**

## 📈 Visualizations

Plots and graphs of actual vs. predicted PM2.5 and PM10 concentrations are included for all cities. These visualizations show strong overlaps indicating high model accuracy.

## 🚧 Challenges Addressed

- Handling non-linear and noisy pollution data
- Lack of consistent or complete data in public datasets
- High variability in PM levels due to urban factors
- Selecting optimal hyperparameters for LSTM

## 🔭 Future Work

- Integrating advanced models like GRU, Transformer, CNN-LSTM
- Deploying models in real-time AQI alert systems
- Expanding study to more cities and pollutants

## 📄 License

This project is licensed under **Creative Commons CC BY-NC-ND 4.0**.  
You are free to share, but must provide attribution, cannot use commercially, and cannot distribute modified versions.

## ✍️ Authors

- [Kedar Desai](#) *(Maintainer)*
- [Pranshu Patel](#)
- [Swara Patel](#)
- [Kanish Shah](#)
- [Samrat Patel](#)
- [Manan Shah](mailto:manan.shah@spt.pdpu.ac.in)
- [Samir Patel](#)

---

## 🔗 Citation

If you use this work, please cite our paper:

> P. Patel et al., “A systematic study on PM2.5 and PM10 concentration prediction in air pollution using machine learning and deep learning model,” *Environmental Chemistry and Ecotoxicology*, vol. 7, pp. 1401–1415, 2025. [DOI:10.1016/j.enceco.2025.07.001](https://doi.org/10.1016/j.enceco.2025.07.001)

---

## 📬 Contact

For collaboration or questions, feel free to reach out to [manan.shah@spt.pdpu.ac.in](mailto:manan.shah@spt.pdpu.ac.in) or open an issue in this repository.


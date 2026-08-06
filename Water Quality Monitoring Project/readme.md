
There is always a first for everything, and I’m excited to share my journey in my first-ever data science competition.  
This experience marked my first exposure to satellite data, and I’m truly grateful for the opportunity to explore it. It was also my first time working with the Snowflake cloud platform, so it was a really exciting experience.

Although I didn’t make it to the Top 10 finalists, I did surpassed the benchmark score set by EY. 
This journey has pushed me to think critically, work with unfamiliar data and strengthen my problem-solving skills. It was a really challenging but highly valuable experience.


## Overview

This project tackles a real-world environmental problem: predicting water quality across rivers in South Africa using satellite and climate data.

The goal was to develop models that can:

- Predict key water quality parameters
- Generalize to unseen locations
- Identify environmental drivers of water pollution

## Problem Statement

Traditional water monitoring is expensive, time-consuming and geographically limited.

This project explores a scalable alternative: Can satellite + climate data be used to predict water quality without physical sampling?

Target variables:

1. Total Alkalinity
2. Electrical Conductance
3. Dissolved Reactive Phosphorus

## Data Sources
Water Quality Data (2011–2015, South Africa)
1. Landsat Satellite Features (spectral bands + indices like NDVI, NDBI, MNDWI)
2. TerraClimate Data (temperature, precipitation, runoff, soil moisture, vapor pressure)

Approach
1. Feature Engineering
- Temporal features: seasonality (sin/cos encoding)
- Spatial features: distance to nearest urban center
- Environmental indicators from satellite indices

2. Models
- Random Forest (baseline)
- XGBoost (strong learner)
- Extra Trees (high variance reduction)

3. Ensemble Learning (Key Highlight)

Implemented a stacking ensemble model:
Base models: RF + XGB + ETR
Meta-model: Ridge Regression
Trained using out-of-fold predictions (OOF) to prevent leakage

Result: Improved generalization on unseen data

## Key Insights
- Water quality shows strong spatial patterns (urban + industrial influence)
- Satellite indices are effective proxies for environmental conditions
- Dissolved phosphorus is harder to predict due to event-driven behavior (runoff, pollution)

## Tech Stack
- Python (Pandas, NumPy, Scikit-learn)
- Satellite data (Microsoft Planetary Computer)
- Snowflake (cloud platform)

## Takeaways

This project demonstrates how:
- Remote sensing + ML can replace traditional monitoring
- Data-driven approaches can support environmental decision-making

## Future Recommendations
- Better handling of temporal gaps
- Feature selection to reduce redundancy
- More advanced models (LightGBM, deep learning)
- Spatial cross-validation for stronger generalization

## Outcome
- Surpassed EY benchmark score
- Built an end-to-end ML pipeline from raw data to predictive modeling

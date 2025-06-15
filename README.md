Fertilizer Recommendation System – Kaggle Playground Series S5E6

This project presents a machine learning model that predicts the **top 3 most suitable fertilizers** for various crop and soil conditions based on climate, nutrient, and soil profile features. It was developed as part of the [Kaggle Playground Series - Season 5, Episode 6](https://www.kaggle.com/competitions/playground-series-s5e6).

Project Goal
To build a model that ranks the top 3 fertilizer recommendations per input case, evaluated using the [Mean Average Precision at 3 (MAP@3)](https://www.kaggle.com/competitions/playground-series-s5e6/overview/evaluation).

📊 Dataset Overview
The dataset includes:
- Numerical Features: Temperature, Humidity, Moisture, Nitrogen, Potassium, Phosphorous
- Categorical Features: Soil Type, Crop Type
- Target: Fertilizer Name (one of 7 classes)

All data is synthetic and licensed under [CC0 (Public Domain)].

⚙️ Model & Approach
- Model Used: LightGBM (with 5-fold stratified cross-validation)
- Pipeline Steps:
  - One-hot encoding for categorical features
  - Label encoding for fertilizer class
  - Column alignment between train and test sets
  - Cross-validation with early stopping
  - MAP@3 submission formatting

📈 Results
The final model produces valid and diverse top-3 fertilizer predictions across test samples and was successfully submitted to the Kaggle leaderboard.


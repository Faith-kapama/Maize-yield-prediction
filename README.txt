
MAIZE YIELD PREDICTION MODEL

Model:
XGBoost regression pipeline for maize yield prediction.

Output:
Predicted maize yield in tonnes per hectare (t/ha).

Required model input features:
1. region
2. season
3. farm_area
4. seed_type
5. irrigation
6. fertilizer_use_clean
7. fertilizer_rate_clean
8. growing_rainfall_mm
9. growing_temperature_c
10. growing_soil_moisture
11. planting_month
12. improved_seed_used
13. traditional_seed_used
14. recycled_seed_used
15. seed_quantity

Files:
- maize_yield_model.joblib
- maize_yield_features.json
- requirements.txt

Validation performance:
MAE ≈ 0.815 t/ha
RMSE ≈ 1.147 t/ha
R² ≈ 0.356

Load model:
    import joblib
    model = joblib.load("maize_yield_model.joblib")

Predict:
    prediction = model.predict(input_dataframe)

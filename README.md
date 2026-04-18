# 📊 Data Science Competition Portfolio

A collection of my competition notebooks covering tabular ML, time series forecasting, and exploratory data analysis.

---

## Datavidia 10 — Jakarta Air Quality Forecasting

📓 [View notebook](Arkavidia%20Datavidia%2010/datavidia-10-air-pollution-prediction.ipynb)

Forecasting daily ISPU air quality categories (BAIK · SEDANG · TIDAK SEHAT) for 5 Jakarta monitoring stations across September–November 2025. I consolidated multi-year ISPU records with daily weather data per station, then performed exploratory analysis to identify historical risk patterns across stations, months, and seasons. The final solution is a transparent rule-based forecasting strategy grounded in those patterns.

---

![Station & Month Risk](Arkavidia%20Datavidia%2010/images/station_month_bars.png)
*TIDAK SEHAT rate by station and month — DKI4 (Lubang Buaya) is historically the most polluted; October carries the highest monthly risk.*

![Category Mix](Arkavidia%20Datavidia%2010/images/category_mix_stacked.png)
*Air quality category distribution per station (Sep–Nov). DKI4 skews heavily toward TIDAK SEHAT while DKI1 (Bundaran HI) is dominated by BAIK days.*

![Season Comparison](Arkavidia%20Datavidia%2010/images/season_comparison.png)
*Dry season (18.2%) sees significantly more TIDAK SEHAT days than wet season (12.2%), driven by stagnant wind and lower rainfall.*

![Heatmap](Arkavidia%20Datavidia%2010/images/station_month_heatmap.png)
*Station × month heatmap of TIDAK SEHAT rate. DKI4 is persistently high-risk; the Sep–Oct window is the peak danger period.*

---

## MCF ITB 2026 — Insurance Claim Cost Prediction

📓 [View notebook](MCF%20Data%20Science%20Competition%202026/mcf.ipynb)

Forecasting monthly individual health insurance claim **frequency**, **severity**, and **total cost** for AXA Financial Indonesia (Aug–Dec 2025) using 4,627 paid claims across 4,096 active policies. The approach covers end-to-end EDA of monthly portfolio trends and mega-claim behavior, followed by causal panel feature engineering with YoY ratios and rolling aggregates. Frequency is modeled with a 5-model ML ensemble (XGBoost, LightGBM, CatBoost, Tweedie GLM, SARIMAX), severity with a 6-model stacking ensemble, and final predictions are adjusted with a YoY bias correction.

---

![Monthly Trends](MCF%20Data%20Science%20Competition%202026/images/monthly_trends.png)
*Monthly claim frequency, severity, and total cost (Jan 2024 – Jul 2025). Severity is declining through mid-2025 while frequency stays relatively stable.*

![Mega Claims](MCF%20Data%20Science%20Competition%202026/images/mega_claims.png)
*Mega-claims (>500M) are rare but account for ~25% of total portfolio cost — modeled separately to prevent outlier distortion.*

![Final Predictions](MCF%20Data%20Science%20Competition%202026/images/final_predictions.png)
*Ensemble predictions for Aug–Dec 2025 with walk-forward MAPE validation of ~16.8% across frequency, severity, and total.*

A collection of my competition notebooks.

---

## Datavidia 10 — Jakarta Air Quality Forecasting

📓 [View notebook](Datavidia%2010/datavidia-10-air-pollution-prediction.ipynb)

Forecasting daily ISPU air quality categories (BAIK · SEDANG · TIDAK SEHAT) for 5 Jakarta monitoring stations across September–November 2025. I consolidated multi-year ISPU records with daily weather data per station, then performed exploratory analysis to identify historical risk patterns across stations, months, and seasons. The final solution is a transparent rule-based forecasting strategy grounded in those patterns.

---

![Station & Month Risk](Datavidia%2010/images/station_month_bars.png)
*TIDAK SEHAT rate by station and month — DKI4 (Lubang Buaya) is historically the most polluted; October carries the highest monthly risk.*

![Category Mix](Datavidia%2010/images/category_mix_stacked.png)
*Air quality category distribution per station (Sep–Nov). DKI4 skews heavily toward TIDAK SEHAT while DKI1 (Bundaran HI) is dominated by BAIK days.*

![Season Comparison](Datavidia%2010/images/season_comparison.png)

*Dry season (18.2%) sees significantly more TIDAK SEHAT days than wet season (12.2%), driven by stagnant wind and lower rainfall.*

![Heatmap](Datavidia%2010/images/station_month_heatmap.png)

*Station × month heatmap of TIDAK SEHAT rate. DKI4 is persistently high-risk; the Sep–Oct window is the peak danger period.*

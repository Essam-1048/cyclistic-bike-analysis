# Cyclistic Bike-Share Case Study (Q1)

**Goal:** Understand how **annual members** and **casual riders** use Cyclistic differently and propose actions to convert casual riders into members.

## Project Structure
```
├── 01_data_cleaning.ipynb
├── 02_analysis.ipynb
├── cyclist_cleaned.csv
├── avg_ride_legth.csv
├── rides_by_day.csv
└── rides_by_month.csv
```

## Summary
This report analyzes Cyclistic trip data (Q1 only) to compare behavior between **annual members** and **casual riders** and to surface actionable marketing recommendations.

## Data & Cleaning
- Source: Public Divvy/Cyclistic trip data (Q1 subset).
- Processed with **pandas**; added `ride_length`, `day_of_week`, and `month`.
- Filtered invalid durations (≤ 0).

## Results (Q1)
- **Total rides analyzed:** 426,677
- **User mix:** members ≈ 378,407 | casual ≈ 48,270
- **Average ride length:** members ≈ 12.7 min | casual ≈ 96.2 min
- **Peak weekday (members):** Tuesday
- **Peak weekday (casual):** Sunday
- **Peak month (members):** January
- **Peak month (casual):** March

## Key Insights
1. **Ride duration gap:** Casual riders typically take longer leisure rides; members take shorter, more utilitarian rides (commutes/errands).
2. **Weekday vs weekend behavior:** Members tend to concentrate rides on weekdays; casual riders skew toward weekends.
3. **Early-year (Q1) trends:** Within Q1 months, usage patterns still show separation by rider type (month and weekday effects).

> NOTE: This analysis is scoped to Q1 data only. Full seasonality requires combining Q2–Q4.

## Recommendations
1. **Weekend-focused offers for casual riders** (e.g., bundled weekend passes, 3-day memberships).
2. **Membership upsell messaging** inside the app after ≥ N rides/month, highlighting cost-per-ride savings.
3. **Commuter retention perks** for members (e.g., ride streak rewards during weekdays).

# Reproducibility
- Cleaned data file: `cyclist_cleaned.csv`
- Summary tables: `avg_ride_legth.csv`, `rides_by_day.csv`, `rides_by_month.csv`
- Notebooks: `01_data_cleaning.ipynb`, `02_analysis.ipynb`

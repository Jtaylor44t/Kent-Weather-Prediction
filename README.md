# Kent-Weather-Prediction
# This takes a dataset and trains a model to predict what the weather will be in the future. Unfortunately I only had about 3 years worth of data so the model would make more accurate predictions if it had more data. This is the output:

==== Target Date Selection ====
Enter the date you want to analyze/predict:
Year (2022-2025) [default: 2025]:  2025
Month (1-12) [default: 4]:  5
Day (1-31) [default: 17]:  1
Hour (0-23) [default: 12]:  10

Selected date: 2025-05-01 10:00
Future time: 2025-05-01 10:00:00

Generating features for future date: 2025-05-01 10:00:00

Training temperature prediction model...
Using features: ['hour', 'dayofweek', 'month', 'year', 'wind_speed', 'humidity', 'pressure', 'cloudcover', 'feelslike', 'uv_index', 'visibility', 'is_day_numeric']
Temperature MSE: 1.3592
Temperature RMSE: 1.1658 degrees

Top 5 most important features for temperature prediction:
      Feature  Importance
8   feelslike    0.992198
4  wind_speed    0.003006
5    humidity    0.001470
6    pressure    0.000907
9    uv_index    0.000619

Predicted Temperature for 2025-05-01 10:00:00: 52.87°F
Predicted Weather Description for 2025-05-01 10:00:00: ["Partly cloudy"]

Top 3 possible weather conditions:
  - Partly cloudy: 75.0%
  - Partly Cloudy : 17.0%
  - Overcast: 4.0%

Finding historical temperatures for 5/1 at 10:00
Filtering from 3939 total records
Found 11 records with month=5, day=1
Searching for data from year 2022...
  Found 3 records for 2022
  Closest match for 2022 at hour 12: temp = 64.0
Searching for data from year 2023...
  Found 4 records for 2023
  Closest match for 2023 at hour 12: temp = 43.0
Searching for data from year 2024...
  Found 4 records for 2024
  Closest match for 2024 at hour 11: temp = 68.0

Temperatures for 5/1 at 10:0:
2022: 64.00°F (closest hour (12))
2023: 43.00°F (closest hour (12))
2024: 68.00°F (closest hour (11))
2025 (Predicted): 52.87°F

Creating temperature visualization...
Visualization saved as 'temperature_trend.png'

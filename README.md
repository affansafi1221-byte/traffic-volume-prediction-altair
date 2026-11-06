

# Traffic Volume Prediction (Altair AI Studio)

Predicts hourly traffic volume using time and weather features,
built as a visual workflow in Altair AI Studio.

## Data
Metro Interstate Traffic Volume (I-94, Minneapolis-St Paul, USA),
2012-2018, 48,204 hourly rows.
Source: UCI Machine Learning Repository
https://archive.ics.uci.edu/dataset/492/metro+interstate+traffic+volume

## Method
1. Created time features from the date: hour and day of week
2. Set traffic_volume as the label
3. Selected features: hour, day of week, temp, rain_1h, snow_1h,
   clouds_all, weather_main
4. Split the data 80/20 into training and test sets
5. Trained a Gradient Boosted Trees model
6. Evaluated predictions on the test set with Performance (Regression)

## Results
Root mean squared error: 1427.343 (on the test set)

## Files
- `process/traffic_prediction.rmp` - Altair AI Studio process
- `screenshots/` - process and performance screenshots

## Screenshots
![Process](screenshots/process.png)
![Performance](screenshots/performance.png)

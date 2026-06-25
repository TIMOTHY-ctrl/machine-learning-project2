# Bee Honey Prediction System

A smart hive monitoring project that uses temperature, humidity, CO2, and bee sound to predict whether honey is present or honey production is in progress.

## Main idea
The system collects sensor data from the honey storage zone of a beehive. It then analyzes patterns such as stable temperature, humidity changes, CO2 rise, and strong buzzing/fanning sound to support honey prediction and harvest decision-making.

## Features
- Temperature monitoring in the honey storage chamber
- Humidity monitoring and volatility analysis
- CO2 monitoring for bee activity and ventilation signals
- Bee sound analysis using frequency features
- Rule-based baseline prediction
- Machine learning model pipeline
- Dashboard-ready demo graphs and reports

## Suggested threshold logic
If temperature stays between 28 C and 35 C, humidity is active around 40% to 65%, CO2 rises around 6,000 to 14,000 ppm, and sound shows strong buzzing/fanning around 150 to 250 Hz, then the system returns Honey present / honey production in progress. Otherwise, it continues monitoring.

## Recommended models
- Random Forest for sensor-based tabular prediction
- SVM for smaller structured datasets
- Gradient Boosting / XGBoost for stronger tabular performance
- CNN or CRNN for audio spectrogram classification

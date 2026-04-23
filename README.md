# Mobile Endpoint Security Analytics & Anomaly Detection

## Overview
This project focuses on Endpoint Detection and Response (EDR) concepts applied to mobile devices. By collecting three days of real-world security logs from a mobile device, this project parses unstructured log data, performs time-series analysis, and applies Machine Learning to detect anomalous security events.

## Key Objectives & Workflow
1. **Data Collection & Parsing:** Extracted 3 days of raw mobile logs (`full_phone_log.log`), cleaning and preprocessing them into structured datasets focusing on event types (e.g., app_launch, network_connection) and sources.
2. **Time-Series Analysis:** Aggregated log events on an hourly basis and calculated rolling averages to establish a baseline of normal mobile device activity.
3. **Machine Learning (Anomaly Detection):** Applied the **Isolation Forest** algorithm from Scikit-Learn to the preprocessed features to automatically detect deviations and potential security anomalies, outputting the results to `anomalies.csv`.
4. **Data Visualization:** Generated time-series plots and heatmaps to visually represent activity spikes and highlight anomalous time frames.

## Technologies Used
- Python
- Pandas (Data Preprocessing & Time-Series Analysis)
- Scikit-Learn (Isolation Forest for Anomaly Detection)
- Matplotlib & Seaborn (Heatmaps and Time-Series Visualization)

# Daikibo Telemetry Data Analysis - Tableau Project

This project analyzes telemetry data from Daikibo factories using Tableau.

## 📊 Visualizations

- **Down Time per Factory**: Shows total downtime (in minutes) per factory.
- **Down Time per Device Type**: Shows downtime by machine type, filtered by selected factory.

## 💡 Logic

A calculated field named **"Unhealthy"** was created in Tableau:
```tableau
IF [Status] = "Unhealthy" THEN 10 ELSE 0 END

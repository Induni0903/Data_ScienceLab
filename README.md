## Project Overview
The primary goal was to analyze historical revenue data from six restaurants (R000–R005) and build a model capable of predicting future earnings while accounting for the significant structural shifts caused by the global pandemic.

## Data Engineering & Enrichment
Exploratory Data Analysis (EDA) revealed that internal data alone could not explain revenue volatility. To improve model accuracy, we enriched the dataset with:

Weather Phenomena: Correlating local weather conditions with dining patterns.

Public Health Data: Identifying the impact of the Covid-19 pandemic on business operations.

Calendar Events: Integrating specific holidays known to influence restaurant traffic.

## Strategic Segmentation
Our analysis identified three distinct business dynamics:

Pre-Covid-19: Stable historical growth.

During Covid-19: High volatility and non-standard behavior.

Post-Covid-19: The current "New Normal."

Decision: To ensure relevance for future predictions, we focused our forecasting model exclusively on the Post-Covid-19 period (December 27th, 2022 – May 3rd, 2023).

## Modeling & Evaluation
We utilized the Prophet forecasting tool to handle seasonality and holiday effects.

Methodology
Iterative Training: Prediction accuracy was computed for +1 day forecasts by iteratively increasing the training set size.

Error Metric: Performance was evaluated using Mean Absolute Percentage Error (MAPE).

Model Selection: The model successfully forecasted earnings for R000, R001, R002, R004, and R005. Restaurant R003 was excluded from the final forecast due to high error variance.

## Results & Future Forecasts
The final phase involved generating a 7-day future forecast (May 4th – May 10th, 2023).

Key Finding: There is a statistically significant increase in earnings during the weekend compared to weekdays across all analyzed restaurants.

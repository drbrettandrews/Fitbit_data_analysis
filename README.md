# Fitbit User Clustering & Sleep Prediction

This project template provides a complete end-to-end workflow for analyzing Fitbit data, clustering users based on behavior, and predicting sleep duration from daily activity metrics. It is designed for reproducibility, portfolio presentation, and educational use.

---

## Project Overview

This analysis leverages Fitbit tracker data to:

- Cluster users based on steps, sedentary time, and sleep duration
- Explore behavioral patterns in physical activity and rest
- Predict total minutes asleep using linear regression on activity data
- Interpret results with clean, report-ready summaries and visualizations

---

## Dataset

**Source:** [Fitbit Fitness Tracker Data on Kaggle](https://www.kaggle.com/datasets/arashnic/fitbit)

- Data includes physical activity, sleep, and sedentary time for 30 users
- Sample files include: `dailyActivity_merged.csv`, `sleepDay_merged.csv`
- Due to size restrictions, raw data is not stored in this repo

---

## Modeling Techniques

### Clustering

- K-means clustering applied to:  
  `TotalSteps`, `SedentaryMinutes`, `TotalMinutesAsleep`
- User behaviors segmented into distinct clusters
- Cluster profiles exported and visualized

### Regression

- Linear regression model:  
  `TotalMinutesAsleep ~ TotalSteps + SedentaryMinutes`
- Performance evaluated using RMSE and R²
- Residuals and predictions visualized for interpretation

---

## Reports & Outputs

- `regression_summary.md` includes full model interpretation
- Residual and prediction plots stored in `/plots/`
- Cluster summaries exported to `/results/`

---

## Technologies Used

- **Language:** R
- **Libraries:** `tidyverse`, `lubridate`, `caret`, `cluster`, `factoextra`, `ggplot2`, `kableExtra`, `knitr`

---

## Author

**Dr. Brett Andrews**  
Dean, School of Business  
Belhaven University  
[LinkedIn](https://www.linkedin.com/in/brett-andrews-4259235) | [Website](https://belhaven.edu)

---

## License

This project is open source under the [MIT License](LICENSE).

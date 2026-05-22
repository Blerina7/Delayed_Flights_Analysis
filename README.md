# Airline Delays Analysis

Exploratory data analysis of U.S. commercial flight delays using the DelayedFlights dataset (Kaggle / U.S. DOT, 2008).

## What this project does

1. Loads and cleans the raw dataset (missing values, outliers, type optimization)
2. Answers 7 research questions with visualizations

## Dataset

Download `DelayedFlightsRaw.csv` from [Kaggle](https://www.kaggle.com/datasets/giovamata/airlinedelaycauses) and place it in the same directory as the notebook.

## Setup

```bash
pip install pandas numpy matplotlib seaborn pyarrow
jupyter notebookb Airline_Delay.ipynb
```

Run all cells in order. The cleaned dataset is saved as `DelayedFlightsClean.parquet`.

## Research Questions

1. Which airlines have the highest average delays, and how does it vary by day of week?
2. What causes large delays (>60 min), and which airports are the main sources?
3. Does the chain effect hold? (`LateAircraftDelay` -> `ArrDelay`)
4. Are long-haul flights more reliable than short ones?
5. Which month has the most cancellations? Is there a seasonal pattern?
6. Do morning flights delay less than evening flights?
7. Do airlines pad their scheduled times to appear more on-time?

## Dependencies

- pandas, numpy, matplotlib, seaborn, pyarrow

## Reference

Dataset: *Airline Delay Causes (2008)*, U.S. DOT Bureau of Transportation Statistics.
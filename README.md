# Purchase Patterns Across Data-Derived Café Demand Regimes

Exploring how café purchase patterns differ across demand regimes identified from transaction data.

This project combines STL decomposition, K-Means clustering, and contrast pattern mining to identify seasonal demand regimes and discover purchase combinations associated with each regime.

## Overview

The analysis follows these steps:

1. Clean and prepare café transaction data.
2. Build a daily demand series using unique transaction receipts.
3. Apply STL decomposition to extract the seasonal demand component.
4. Use K-Means clustering to identify higher and lower seasonal demand regimes.
5. Assign demand regimes to individual transactions.
6. Construct transaction-level shopping baskets.
7. Identify and compare emerging purchase patterns across regimes.

## Repository Contents

| File | Description |
|------|-------------|
| Purchase Patterns_Across_Data_Derived_Café_Demand_Regimes.ipynb | Main notebook containing data preparation, demand analysis, pattern mining, and visualizations. |

> The transaction dataset is included in this repository.

## Technologies

- Python
- pandas
- NumPy
- Matplotlib
- statsmodels
- scikit-learn
- Google Colab / Jupyter Notebook

## Dataset

The analysis requires a transaction-level CSV containing information used to identify:

- Transaction dates
- Unique receipts
- Purchased items
- Item groups

Review the notebook's data preparation cells for the exact column names and expected format.

## Analysis Outputs

The notebook produces:

- Daily demand visualizations
- STL decomposition components
- Demand regime characteristics and comparisons
- Demand regime distributions over time
- Transaction baskets grouped by regime
- Emerging purchase patterns for higher and lower seasonal demand
- Pattern comparisons by itemset size
- Final purchase pattern summary tables

## Interpretation

Demand regimes are derived from the seasonal component of daily demand. They describe relative seasonal demand conditions within the analyzed dataset.

Purchase patterns highlight item combinations associated with each regime. Results depend on the input data, preprocessing choices, and mining thresholds.

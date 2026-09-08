# Optimizing Supply Chain Logistics: A Data Driven Approach to Inventory Management and Demand Forecasting

## IDRA Final Capstone Project

This project analyzes supply chain data to understand demand patterns, inventory conditions, and factors affecting product movement. A time aware machine learning approach is also used to predict daily demand and support inventory planning.

### Project Overview

The project covers the main stages of a data science workflow:

- Data understanding and quality checks
- Data cleaning and preprocessing
- Exploratory data analysis and visualization
- Statistical analysis
- Feature engineering
- Demand prediction using machine learning
- Model evaluation
- Business findings and recommendations

### Dataset

The project uses the supply chain dataset provided for **IDRA Capstone Project 3**.

The dataset contains **91,250 records and 15 columns**, covering daily observations from 2024. Important variables include sales, inventory levels, supplier lead time, reorder points, order quantities, pricing, promotions, and demand forecasts.

The modelling target is **`Units_Sold`**, used as a daily demand proxy.

### Machine Learning

Several baselines and regression models were evaluated using a chronological train-test split. The final selected model is **HistGradientBoostingRegressor**.

Test performance:

| Metric | Result |
|---|---:|
| MAE | 2.193 |
| RMSE | 2.753 |
| R² | 0.793 |

The existing `Demand_Forecast` variable was also evaluated as a baseline and is treated as a planning-time forecast for modelling purposes.

### Project Structure

```text
Supply-Chain-Logistics/
│
├── Capstone_Supply_Chain_Notebook.ipynb
├── Supply_Chain_Capstone_Report.pdf
├── P_3_supply_chain_dataset1.csv
├── supply_chain_cleaned_dataset.csv
└── README.md
```

### Running the Project

Open `Capstone_Supply_Chain_Notebook.ipynb` in Jupyter Notebook or Google Colab and keep `P_3_supply_chain_dataset1.csv` available in the working directory.

Run the notebook from beginning to end. The notebook performs the analysis and generates the supporting CSV outputs in an `outputs/` folder.

### Requirements

The notebook uses standard Python data science libraries, including:

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

### Note

This repository contains the supporting files for the IDRA Final Capstone Project. The detailed methodology, analysis, findings, limitations, and recommendations are documented in the project report.

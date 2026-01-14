# US Honey Production Trend Analysis

Exploratory data analysis of US honey production from 1995 to 2021, focusing on how production volumes and prices have changed over time across different states.

## Overview

This project analyzes a honey production dataset containing yearly statistics for US states, including colonies, yield per colony, total production, stocks, average price, and value of production. The goal is to understand long-term trends in honey output and pricing, and how different states contribute to total national production. [file:11]

## Dataset

- **Source:** US honey production dataset (CSV), originally shared via Google Drive.  
- **Rows:** 1,115 records (state–year combinations). [file:11]  
- **Key columns:** [file:11]  
  - `state`: US state name  
  - `colonies_number`: Number of honey bee colonies  
  - `yield_per_colony`: Yield per colony (pounds)  
  - `production`: Total honey production (pounds)  
  - `stocks`: Stocks held by producers (pounds)  
  - `average_price`: Average price per unit  
  - `value_of_production`: Total value of honey produced  
  - `year`: Calendar year  

> Note: The dataset file name in the notebook is `US_honey_dataset (1).csv`. Update the path if you store it in a different folder. [file:11]

## Objectives

- Inspect and understand the structure and summary statistics of the dataset. [file:11]  
- Analyze how total honey production has changed over time in the US. [file:11]  
- Examine trends in average honey price over the years. [file:11]  
- Compare production across states for selected years (e.g., 2000 vs. 2021). [file:11]

## Methods and Analysis

The notebook includes the following steps:

- **Data loading and inspection**  
  - Load the CSV into a Pandas DataFrame.  
  - View head, shape, and descriptive statistics for numeric columns. [file:11]

- **Data cleaning and preparation**  
  - Drop or ignore unnecessary index-like columns such as `Unnamed: 0`. [file:11]  
  - Check for missing values and basic data consistency.

- **Exploratory data analysis (EDA)**  
  - Distribution analysis of colonies, yield per colony, production, and prices. [file:11]  
  - Group-by operations to compute total production per year for the entire US. [file:11]  
  - Aggregation of average price per year to observe pricing trends. [file:11]  
  - State–year production views to see which states dominate production. [file:11]

- **Visualization**  
  - Line plots of total US honey production by year. [file:11]  
  - Line plots of average honey price by year. [file:11]  
  - Additional plots (e.g., bar plots or heatmaps) to compare states for specific years. [file:11]

## Tech Stack

- **Language:** Python 3  
- **Libraries:**  
  - `pandas` and `numpy` for data manipulation  
  - `matplotlib` and `seaborn` for visualizations [file:11]  
- **Environment:** Jupyter / Google Colab [file:11]

## How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/us-honey-production-analysis.git
   cd us-honey-production-analysis

2. Create and activate a virtual environment (optional but recommended):
   python -m venv .venv
   source .venv/bin/activate   # On Windows: .venv\Scripts\activate

3. Install dependencies:
   pip install -r requirements.txt

4. Place the dataset file in the project folder (for example: data/US_honey_dataset.csv) and      update the path in the notebook if needed.

5. Open the notebook:
   Jupyter Notebook 8_casestudy_honeyproduction.ipynb
   or upload it to Google Colab and adjust the CSV path (e.g., /content/US_honey_dataset (1).csv). 
7. 

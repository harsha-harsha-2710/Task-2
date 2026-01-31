# Task 2: Data Cleaning & Missing Value Handling

## Project Overview
In this phase of the internship, the focus shifted from data exploration to **Data Preprocessing**. The goal was to handle "dirty" data by identifying, visualizing, and resolving missing values using various imputation techniques. This ensures the dataset is robust and ready for Machine Learning models without losing valuable information.

## Objectives & Steps
1. **Missing Data Audit:** Used `.isnull().sum()` to quantify the extent of missing information across features.
2. **Visual Analysis:** Created bar charts and heatmaps to identify patterns in data gaps (e.g., whether data is missing at random).
3. **Numerical Imputation:** Applied **Median Imputation** for continuous variables to ensure the central tendency is maintained without being skewed by outliers.
4. **Categorical Imputation:** Implemented **Mode Imputation** for string-based or classification columns.
5. **Feature Pruning:** Established a threshold (40%) to remove columns with excessive missingness that could introduce significant bias.
6. **Validation:** Conducted a post-cleaning audit to verify a 0% null-rate across the final dataset.

## Technical Implementation
* **Language:** Python
* **Library:** Pandas (for data manipulation), NumPy (for numerical operations)
* **Visualization:** Matplotlib / Seaborn
* **Techniques:** Median/Mode Imputation, Column Dropping, Statistical Validation

## Key Observations
* **Imputation Choice:** Median was chosen over Mean for numerical data to provide better resistance against the influence of outliers in the "House Prices" / "Medical" datasets.
* **Data Integrity:** By cleaning the data rather than simply deleting rows, I preserved the dataset's volume, which is critical for model training.
* **Quality Improvement:** The dataset moved from an incomplete state to a "Model-Ready" state while maintaining the original statistical distribution.

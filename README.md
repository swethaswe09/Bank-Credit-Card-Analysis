# AtliQo Bank - A/B Test Analysis (Phase 2)

A statistical analysis of an A/B test campaign conducted by AtliQo Bank. This project is Phase 2 of the analysis, following Phase 1, which identified the **18–25 age group** as the target market.

## Objective

The objective is to determine whether the new credit card marketing campaign **increased the average transaction amount** among the target 18–25 age group compared with the control group.

## Methodology

A **one-tailed z-test for two independent samples** was used to compare the average transaction amounts of the test and control groups.

### Hypotheses

* **Null Hypothesis (H₀):** The average transaction amount of the test group is less than or equal to the control group.
* **Alternative Hypothesis (H₁):** The average transaction amount of the test group is greater than the control group.
* **Significance Level (α):** 0.05 (5%)

## Data

The analysis uses `avg_transactions_after_campaign.csv`, which contains the daily average transaction amounts for both the control group and the test group after the campaign launch.

## Analysis

The transaction distributions of the control and test groups were visualized using **Matplotlib and Seaborn** to understand the difference in their distributions and average transaction amounts.

The hypothesis test was then performed using `statsmodels.stats.ztest`.

## Results

* **Z-statistic:** 2.748
* **P-value:** 0.00299
* **Significance Level:** 0.05

Since the **p-value (0.00299) is less than 0.05**, the null hypothesis is rejected.

### Conclusion

The results are statistically significant and provide evidence that the new credit card marketing campaign **increased the average transaction amount among customers in the 18–25 age group** compared with the control group.

## Technologies Used

* **Python** — Statistical analysis and data processing
* **Jupyter Notebook** — Analysis environment
* **Pandas** — Data loading and manipulation
* **Statsmodels** — One-tailed z-test
* **Matplotlib** — Data visualization
* **Seaborn** — Distribution visualization

## How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd <repository-folder>
```

### 2. Install the required libraries

```bash
pip install pandas statsmodels matplotlib seaborn jupyterlab
```

### 3. Add the dataset

Ensure `avg_transactions_after_campaign.csv` is present in the same directory as the notebook.

### 4. Run the notebook

Open `Testing for new Credit Card.ipynb` using Jupyter Notebook or JupyterLab and run the cells.

## Key Takeaway

This project demonstrates how **hypothesis testing and statistical significance** can be used to evaluate the effectiveness of a marketing campaign and support data-driven business decisions.


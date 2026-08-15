# Bank-Credit-Card-Analysis

This project is a statistical analysis of an A/B test campaign conducted by AtliQo Bank. It serves as Phase 2, following the initial target market identification (18-25 age group) from Phase 1.

Objective
The objective of this analysis is to statistically determine if the new credit card, which was marketed to the target "test group," successfully increased their average transaction amount compared to the "control group".

Methodology: Hypothesis Testing
A one-tailed z-test for two independent samples was used to compare the means of the two groups.

Null Hypothesis (
H
0
): The average transaction amount of the test group is less than or equal to the average transaction amount of the control group.
Alternative Hypothesis (
H
1
): The average transaction amount of the test group is greater than the average transaction amount of the control group.
Significance Level (
α
): 0.05 (or 5%).
Data
The analysis uses the avg_transactions_after_campaign.csv file, which contains the daily average transaction amounts for both the control group and the test group (the 18-25 age market) after the campaign launch.

Visualizing the Distributions
Below are the distributions of the average transaction amounts for both the control and test groups. This visualization helps to intuitively understand the difference in means that the hypothesis test quantifies.

Distribution of Control and Test Group Transaction Amounts

Results & Conclusion
The statsmodels.stats.ztest was performed to get the test statistic and p-value.

Z-statistic: 2.748
P-value: 0.00299
Conclusion: Reject the Null Hypothesis.

Since the p-value (0.00299) is less than the significance level (0.05), we reject the null hypothesis. The results are statistically significant, and we can conclude that the marketing campaign for the new credit card successfully increased the average transaction amount for the 18-25 age group.

Technologies Used
Python
Jupyter Notebook
Pandas: For data loading and manipulation.
Statsmodels: For performing the one-tailed z-test.
Matplotlib & Seaborn: For data visualization.
How to Run This Project
Clone the repository.
Install the required libraries:
pip install pandas statsmodels matplotlib seaborn jupyterlab
Ensure the avg_transactions_after_campaign.csv data file is in the same directory as the notebook.
Run the Testing for new Credit Card.ipynb file using JupyterLab or Jupyter Notebook.

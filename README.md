# Lab 6: Association Rule Mining with Apriori and FP-Growth

**Author:** Jacob Jeffers  
**Course:** MSCS 634 – Data Mining  
**Lab Title:** Discovering Frequent Itemsets and Rules with the Online Retail Dataset

## Purpose

This lab focused on applying association rule mining techniques using both the Apriori and FP-Growth algorithms. The goal was to identify frequent item combinations in transaction data and generate rules that reveal useful relationships.

## What I Did

- Cleaned and preprocessed the Online Retail dataset
- Transformed the data into a format compatible with Apriori and FP-Growth
- Used `mlxtend` to apply both algorithms and extract frequent itemsets
- Generated association rules using confidence and lift thresholds
- Visualized item frequency and rule strength using bar plots and scatter plots

## Key Insights

- FP-Growth performed much faster than Apriori, especially with larger datasets
- Both algorithms identified strong associations between common item pairs
- Scatter plots showing lift vs. confidence helped highlight the most promising rules
- I saw how rule metrics like support, confidence, and lift work together to judge rule strength

## Trouble Areas

One of the initial challenges was preparing the dataset in the right format for the algorithms. I had to group items by invoice and encode the data using `TransactionEncoder` before mining itemsets. Apriori also took longer to run, especially with lower support values. Adjusting the support threshold helped find a balance between runtime and meaningful output.

## Files Included

- `lab6.ipynb`: Jupyter Notebook with all code, outputs, and visuals
- `README.md`: Summary of the lab work and findings

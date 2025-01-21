# Hypothesis-Testing-in-Healthcare

This project involves analyzing a dataset from GlobalXYZ, a pharmaceutical company that conducted a randomized controlled drug trial. The focus is on examining adverse effects related to a drug versus a placebo. The goal is to determine if the adverse effects are of significant proportions between the Drug and Placebo groups, helping to assess the safety of the drug.

Steps Taken:
Data Import:

Loaded the dataset drug_safety.csv using pandas and imported necessary packages: numpy, seaborn, statsmodels, and pingouin for data manipulation, visualization, and statistical tests.
Adverse Effects Analysis:

Grouped data by trx (treatment) and counted the number of occurrences of the adverse_effects (Yes/No) for both the Drug and Placebo groups.
Calculated the total number of adverse effects in each treatment group.
Proportions Z-Test:

Performed a two-sample z-test to compare the proportions of participants reporting adverse effects between the Drug and Placebo groups to assess statistical significance.
Chi-Square Test for Independence:

Conducted a chi-square test to determine if the number of adverse effects (num_effects) is independent of the treatment group (trx). This helps understand if the drug impacts the severity (number) of adverse effects.
Age Distribution Visualization:

Plotted a histogram of age distributions for both the Drug and Placebo groups to visualize any age differences between the groups.
Normality Test:

Conducted the Shapiro-Wilk normality test to assess whether the age data for both groups follows a normal distribution, which influences the choice of statistical test.
Mann-Whitney U Test:

Since age data was not normally distributed, a non-parametric Mann-Whitney U test was used to compare the age distributions between the two groups.
Outcomes:
Z-Test: The p-value from this test helped determine if the difference in adverse effects between the Drug and Placebo groups was statistically significant.
Chi-Square Test: The p-value from the chi-square test assessed if the number of adverse effects was influenced by the treatment group.
Mann-Whitney U Test: The test provided insights on whether there was a significant difference in the age distribution between the two groups.
This analysis helps determine the drug's safety by evaluating adverse reactions and demographic factors, contributing to evidence-based decision-making regarding the drug's use.

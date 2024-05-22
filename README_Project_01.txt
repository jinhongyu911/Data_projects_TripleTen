Project_01 - EDA & HT (Mobile)

Project Description
The telecom operator Megaline offers its clients two prepaid plans, Surf and Ultimate.
The commercial department wants to know which of the plans brings in more revenue in order to adjust the advertising budget.
Carry out a preliminary analysis of the plans based on a relatively small client selection.
You'll have the data on 500 Megaline clients: who the clients are, where they're from, which plan they use, and the number of calls they made and text messages they sent in 2018.
Your job is to analyze the clients' behavior and determine which prepaid plan brings in more revenue.

Goal
Analyze the datasets and advise on which of the plans brings in more revenue in order to adjust the advertising budget.

Taks Performed
1. Load necessary packages and datasets
2. EDA
* Check and correct datatypes
* Check and eliminate duplicate values
* Fill missing values
* Feature engineering
* Merge datasets into a single dataset
* Visualize the data (histogram, boxplots) to find seasonal trends and insights
3. Hypothesis Testing
* State the null hypothesis and significance level (alpha)
* Perform the hypothesis tests, then accept or reject the null hypothesis

Conclusions
1. surf:  339 users (total 1180 months)	 ultimate: 161 users (total 579 months)
2. The total revenue from 'surf' users is higher than 'ultimate' users given the higher user & month counts. But the average revenue from the 'ultimate' users are ~20% higher than 'surf' users.
3. Hence, I recommend allocating more of the advertising budget to the 'ultimate' plan to increase revenue.
   But this will also depend on the advertising ROI or the average acquisition cost for a new 'ultimate' user vs 'surf' user.
4. Given the most revenue for the 'surf' package comes from the internet overcharges (~2x the package price), increasing the 'usd_per_gb' price could lead to increase in per user total revenue for 'surf' package.
5. In Feb and March, 'ultimate' plan users  average call duration and internet usage are significantly higher than 'surf' plan users.
   This could be further investigated to see if there are any underlying reasons for this.

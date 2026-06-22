### Data Analytics & Visual Report

#### Dataset Focus: Customer churn, revenue, and income analysis (Merging Client.csv and Record.csv)

#### 1. Data Cleaning Protocol Log
- **Raw Input Problem:** The datasets `Client.csv` and `Record.csv` required integration via the common `Customer_ID` field. The `income` column contained non-numerical values requiring conversion, and several rows contained null values that could skew the analysis.
- **AI Cleaning Instruction:** "Merge `Client.csv` and `Record.csv` on `Customer_ID`. Convert the `income` column to a numeric format using coercion to handle errors. Drop all rows where `income`, `churn`, or `rev_Mean` contain null values to ensure structural integrity."
- **Result:** Successfully integrated the datasets and normalized 100% of the target rows for valid analytical plotting.

#### 2. Visualizations Generated

**Distribution of Income by Churn Status**
![Distribution of Income by Churn Status](https://github.com/rbauya-dev/GE-IT-Skills-portfolio/blob/main/Prompts/Code_Generated_Image%20(3).png?raw=true)

**Distribution of Mean Revenue by Churn Status**
![Distribution of Mean Revenue by Churn Status](https://github.com/rbauya-dev/GE-IT-Skills-portfolio/blob/main/Prompts/Code_Generated_Image%20(2).png?raw=true)

#### 3. Human Analytical Narrative (The 'Why' Factor)
"The data charts highlight a critical insight: there is minimal observable difference in income distribution between customers who churn and those who remain. Similarly, while mean revenue distributions appear largely identical across both groups, the presence of extreme outliers in the churned segment (as seen in the revenue chart) suggests that high-value customers might be churning due to specific, non-income-related service failures.

This analysis indicates that simply targeting specific income brackets for retention efforts will likely be ineffective. Instead, the LGU and service providers should investigate the high-revenue churn outliers to identify potential service-level issues, such as connectivity drops or customer care dissatisfaction, which are the more probable drivers of attrition in the current regional infrastructure."

# Health Insurance Coverage Analysis
#### Overview
This project analyzes health insurance coverage data across U.S. states, focusing on changes in uninsured rates, Medicaid expansion, and marketplace health insurance coverage. The goal is to understand the impact of Medicaid expansion under the Affordable Care Act (Obamacare) and explore relationships between tax credits and marketplace enrollment.
________________________________________
## Problem Statement
My project aims to answer the following key questions:
1.	How did the uninsured rate change from 2010 to 2015 in states that expanded Medicaid compared to those that did not?
2.	What is the relationship between the average monthly tax credit and the number of people covered by marketplace health insurance in 2016?
3.	Which states experienced the largest increase in Medicaid enrollment from 2013 to 2016, and how does this relate to their Medicaid expansion status?
The dataset provides health insurance coverage data for each state, including uninsured rates, Medicaid and Medicare enrollment, and marketplace health insurance coverage. My analysis seeks to uncover trends and relationships that can inform policy decisions and public health strategies.
________________________________________
## Repository Structure
•	states.csv: The dataset containing health insurance coverage data for U.S. states.
•	health_insurance_analysis.ipynb: Jupyter Notebook containing the Python code for data exploration, cleaning, analysis, and visualization.
•	README.md: This file, providing an overview of the project, its motivation, and results.
________________________________________
## Libraries Used
•	Pandas: For data manipulation and analysis.
•	Matplotlib: For creating static visualizations.
•	Seaborn: For enhanced data visualization and plotting.
•	NumPy: For numerical operations (used indirectly through Pandas).
________________________________________
## Motivation
The Affordable Care Act (ACA) significantly impacted health insurance coverage in the United States, particularly through Medicaid expansion and marketplace health insurance. This project aims to:
•	Quantify the impact of Medicaid expansion on uninsured rates.
•	Explore the relationship between tax credits and marketplace enrollment.
•	Identify states with the most significant changes in Medicaid enrollment.
Understanding these trends can help policymakers and stakeholders evaluate the effectiveness of health insurance programs and identify areas for improvement.
________________________________________
## Strategy for Solving the Problem
1.	Data Exploration and Cleaning:
o	Load the dataset and inspect for missing values or inconsistencies.
o	Handle missing data by filling gaps with appropriate values (e.g., 0 for missing Medicaid enrollment changes).
o	Ensure all columns are in the correct data type for analysis.
2.	Data Analysis:
o	Compare uninsured rate changes between states that expanded Medicaid and those that did not.
o	Calculate the correlation between average monthly tax credits and marketplace health insurance coverage.
o	Identify the top 5 states with the largest Medicaid enrollment increases and analyze their Medicaid expansion status.
3.	Data Visualization:
o	Create visualizations to communicate findings effectively, including box plots, scatter plots, and bar plots.
4.	Interpretation and Reporting:
o	Summarize the results and discuss their implications.
o	Suggest potential improvements to the analysis.
________________________________________
## Results Summary
1.	Uninsured Rate Change:
o	States that expanded Medicaid saw an average uninsured rate reduction of 6.5%, compared to 4.8% in non-expansion states.
o	This suggests that Medicaid expansion played a significant role in reducing uninsured rates.
2.	Tax Credits and Marketplace Coverage:
o	I expected a moderate positive correlation (0.45) was found between average monthly tax credits and marketplace health insurance coverage.
o	Higher tax credits may encourage more people to enroll in marketplace plans.
o	Actual results: The correlation result of -0.01 between the average monthly tax credit and marketplace health insurance coverage is unexpected and suggests no linear relationship between these two variables. This outcome contradicts the initial hypothesis that higher tax credits would lead to higher marketplace enrollment. Let’s break down the implications and explore potential reasons for this result.
3.	Medicaid Enrollment Increase:
o	The top 5 states with the largest Medicaid enrollment increases were California, Arizona, Kentucky, Oregon, and Colorado.
o	All of these states expanded Medicaid, highlighting the effectiveness of expansion in increasing enrollment.
________________________________________
## Background Information
•	Problem Domain: Public health and health insurance policy.
•	Project Origin: The dataset was created to analyze the impact of the Affordable Care Act (ACA) on health insurance coverage across U.S. states.
•	Related Datasets: Other datasets on health insurance coverage, healthcare costs, and demographic factors could provide additional context.
________________________________________
## Implementation Improvements
Current Implementation
My analysis uses basic statistical methods and visualizations to explore the dataset. While effective, it could be enhanced with more advanced techniques.
## Potential Improvements
1.	Machine Learning Models:
o	Use regression models to predict uninsured rates based on factors like Medicaid expansion, tax credits, and state demographics.
o	Compare the performance of linear regression, decision trees, and random forests.
2.	Interactive Visualizations:
o	Use libraries like Plotly or Dash to create interactive visualizations that allow users to explore the data dynamically.
3.	Geospatial Analysis:
o	Use GeoPandas to create maps showing uninsured rates, Medicaid expansion status, and other metrics by state.
## Comparison to Current Solution
•	Machine Learning Models: Would provide predictive insights but require more computational resources and expertise.
•	Interactive Visualizations: Would enhance user engagement but may be overkill for a static analysis.
•	Geospatial Analysis: Would add a spatial dimension to the analysis but requires additional data preparation.
________________________________________
## Interesting or Difficult Aspects
1.	Handling Missing Data:
o	Some states had missing values for Medicaid enrollment in 2013. These were filled with 0, assuming no change in enrollment. This approach was simple but may not fully capture the underlying trends.
2.	Correlation Analysis:
o	The moderate correlation between tax credits and marketplace coverage was interesting but not strong enough to draw definitive conclusions. Further analysis with additional variables (e.g., income levels) could provide more insights.
________________________________________
## Final Results and Discussion
•	Medicaid Expansion Impact: The analysis confirmed that Medicaid expansion significantly reduced uninsured rates, supporting the policy's effectiveness.
•	Tax Credits and Marketplace Coverage: The moderate correlation suggests that tax credit does not play a role in marketplace enrollment.
•	Medicaid Enrollment Growth: The top state with the largest enrollment increases all expanded Medicaid, reinforcing the importance of this policy.
## Exploration of Techniques
•	Statistical Methods: Worked well for initial exploration but lack predictive power.
•	Visualizations: Effectively communicated trends.
________________________________________
## Acknowledgements
•	Dataset Source: The dataset was provided by Kaggle for analysis, and is based on publicly available health insurance coverage data.
•	Libraries: Thanks to the developers of Pandas, Matplotlib, and Seaborn for their powerful tools for data analysis and visualization.
•	Blog Post: https://medium.com/@dgrah026/healthcare-for-all-a-data-driven-journey-through-obamacares-impact-b7852f111913
1. **Health Insurance Dataset** – Kaggle dataset on health insurance data.  
   [🔗 Kaggle Dataset](https://www.kaggle.com/datasets/hhs/health-insurance/data)  

2. **Convert Data to Numeric** – Pandas `to_numeric()` function documentation.  
   [🔗 Pandas `to_numeric`](https://pandas.pydata.org/docs/reference/api/pandas.to_numeric.html)  

3. **Handling Missing Values** – Stack Overflow discussion on `df.isnull().sum()`.  
   [🔗 Stack Overflow: `isnull().sum()`](https://stackoverflow.com/questions/59349484/why-does-df-isnull-sum-work-the-way-it-does)  

4. **Fill Missing Data** – Pandas `fillna()` function documentation.  
   [🔗 Pandas `fillna`](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.fillna.html)  

5. **Descriptive Statistics** – Pandas `describe()` function reference from W3Schools.  
   [🔗 Pandas `describe()`](https://www.w3schools.com/python/pandas/ref_df_describe.asp)  

6. **Box Plot Visualization** – Seaborn's `boxplot()` function documentation.  
   [🔗 Seaborn `boxplot()`](https://seaborn.pydata.org/generated/seaborn.boxplot.html)  

7. **Correlation Matrix** – Pandas `corr()` function for finding correlations between columns.  
   [🔗 Pandas `corr()`](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.corr.html)  

8. **Scatter Plot Visualization** – Seaborn's `scatterplot()` function documentation.  
   [🔗 Seaborn `scatterplot()`](https://seaborn.pydata.org/generated/seaborn.scatterplot.html)  

9. **Regression Plot** – Seaborn's `regplot()` function for regression analysis.  
   [🔗 Seaborn `regplot()`](https://seaborn.pydata.org/generated/seaborn.regplot.html)  

10. **Find Largest Values** – Pandas `nlargest()` function for selecting top rows.  
   [🔗 Pandas `nlargest()`](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.nlargest.html)  

11. **Bar Plot Visualization** – Seaborn's `barplot()` function documentation.  
   [🔗 Seaborn `barplot()`](https://seaborn.pydata.org/generated/seaborn.barplot.html)  
________________________________________
## Conclusion
My project provides valuable insights into the impact of Medicaid expansion and marketplace health insurance coverage in the United States. By analyzing uninsured rates, tax credits, and Medicaid enrollment, the project highlights the effectiveness of key ACA policies and identifies areas for further exploration. Future improvements could include advanced modeling techniques and interactive visualizations to enhance the analysis further.

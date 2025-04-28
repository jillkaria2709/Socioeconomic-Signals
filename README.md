# Analysis of Income, Inflation, Expenditure, and Crime Across U.S. States (2012–2022)

## Project Overview
This project explores how economic conditions—specifically income, inflation, and personal expenditure—relate to violent crime rates across U.S. states from 2012 to 2022. Using Python, we collected, cleaned, merged, and analyzed both structured (CSV) and semi-structured (JSON) data to derive insights through statistical analysis and dynamic visualizations.

This project was completed as part of **IST652 - Scripting for Data Analysis**

## Team
- **Jill Karia** 
- **Shivani Pandeti** 
- **Reeya Tapan Patra** 

## Data Sources
- **Personal Income Data** ([BEA](https://apps.bea.gov/regional/downloadzip.ht))  
  *File:* `SAINC1__ALL_AREAS_1929_2024.csv`
- **Inflation Data** ([BEA](https://apps.bea.gov/regional/downloadzip.ht))  
  *File:* `SASUMMARY__ALL_AREAS_1998_2024.csv`
- **Personal Consumption Expenditure Data** ([BEA](https://apps.bea.gov/regional/downloadzip.ht))  
  *File:* `SAPCE1__ALL_AREAS_1997_2023.csv`
- **Violent Crime Data** ([FBI Crime Data Explorer API](https://catalog.data.gov/dataset?tags=crime))  
  *Format:* JSON (via REST API)

## Preprocessing Summary
- Cleaned and reshaped all datasets into a **State | Year** format.
- Filtered necessary indicators (GDP, Income, RPPS, Unemployment, Crime rates).
- Adjusted expenditures for inflation using RPPS indices.
- Merged datasets based on State and Year.
- Final dataset: ~561 records covering all 50 states + D.C. across 11 years.

## Research Questions
1. How do state-level income and inflation trends correlate with changes in overall consumer expenditure over the past decade?
2. How does spending behavior differ between high-income and low-income groups within a state when adjusted for inflation?
3. Which states show the strongest correlation between income changes and changes in property/violent crime rates?
4. Is there a significant difference in crime rates between states with high inflation and low income versus states with low inflation and high income?
5. How does spending behavior differ between high-income and low-income groups when adjusted for inflation?
6. How does the volatility of states' unemployment behavior look like over the years?


## Methods and Tools
- **Programming Language:** Python
- **Libraries Used:** Pandas, NumPy, Plotly, Seaborn, Scikit-learn
- **Techniques:**
  - Data Cleaning and Transformation
  - API Data Retrieval
  - Regression Analysis (OLS)
  - Cluster Analysis (K-Means, PCA)
  - Interactive Visualizations (Line plots, Scatter plots, Choropleth maps, Animated charts)


## Key Outputs
- Line plots showing income and expenditure trends.
- Regression summaries analyzing correlations.
- Stacked bar charts of expenditure categories.
- Choropleth maps for crime dominance and correlations.
- Animated bar charts visualizing income vs. expenditure gaps.
- Cluster visualizations of unemployment volatility.


## Conclusion
Our project highlighted key economic and social patterns across U.S. states, showing:
- Strong positive correlations between income and expenditure.
- Differences in spending behavior based on income levels.
- Correlations between economic stress and higher crime rates.
- States' varied resilience to unemployment shocks.

These findings provide a foundation for further studies on economic resilience and public policy planning.


## How to Run
1. Install Python libraries:
```bash
pip install pandas numpy plotly seaborn scikit-learn requests
```
2. Download datasets or fetch via API as described.
3. Run the scripts sequentially to preprocess, merge, analyze, and visualize the data.
4. View saved outputs (interactive HTML files for dynamic plots).


## Acknowledgments
- U.S. Bureau of Economic Analysis (BEA)
- FBI Crime Data Explorer
- Syracuse University, School of Information Studies

---

*This project was completed for educational purposes only.*

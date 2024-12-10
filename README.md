# CANDY MARKET SHARE ANALYSIS



## Project Overview
The objective of this Power BI report is to analyze and visualize comprehensive market data from a leading European market research company specializing in the confectionery industry. The dataset includes detailed information on major manufacturers, their brands, packaging, and sales volumes in a specific regional market.

## Problem Statement
Over the past two years, the confectionery market has witnessed significant shifts in sales dynamics and consumer preferences. A leading European market research company seeks to leverage a data-driven approach to understand the current market landscape and its evolution between 2022 and 2023. The objective is to provide actionable insights that will support strategic decision-making for major manufacturers in the confectionery industry.

## Process
`Data Preparation`
- The initial phase involved performing data cleaning tasks, including the removal of null values, the elimination of unnecessary columns, handling duplicates, and adjusting data types to ensure data quality.

`Data Modeling`
- The subsequent step was to create calculated measures and tables using DAX (Data Analysis Expressions) in Power BI, enhancing the dataset's analytical capabilities.

<pre><code>
  # Calculated Total Sales 
Total Sales = SUM('Table3'[SALES VOLUME  in EUR])
 
  # Created Year-Over-Year Sales to compare sales performance from 2022 to 2023
 YoY Sales = 
CALCULATE(
    [Total Sales],
    SAMEPERIODLASTYEAR(Table3[Date])
)
  
  # Calculated Year-Over-Year Growth Rate
 YoY Growth Rate = 
DIVIDE(
    ([Total Sales] - [YoY Sales]),
    [YoY Sales]
)
</code></pre>

`Data Analysis`
- Following data modeling, an in-depth data analysis was conducted within Power BI, utilizing various visualization techniques like matrices to identify trends in sales, category-wise performance, manufacturer details, and product insights. This analysis provided actionable insights into market dynamics and supported strategic decision-making.

`Dashboard Creation`
- The project proceeded with the development of an interactive and dynamic dashboard in Power BI. This dashboard was designed to include bookmark features and filters, allowing for seamless navigation and personalized views across various charts and visualizations. These tools provided a more comprehensive and tailored view of the data, enhancing the overall user experience.


## Dashboard 
The dashboard section offers an array of visualizations that empower users to explore and understand sales data. Key features of the dashboard include:

- Visualization of Monthly and Yearly Sales Trends: Interactive charts showcasing sales trends over different periods.
- Comparison of Sales Across Different Categories: Detailed comparisons of sales by product type, packaging type, manufacturer, brands, items, and distribution channels.
- KPIs: Key Performance Indicators such as revenue, sales volume, year-over-year sales, year-over-year growth rate, and items sold.

()

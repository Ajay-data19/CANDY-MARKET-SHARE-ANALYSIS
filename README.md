# Confectionery Market Share Analysis
![confectionery-industry-typographic-header-delicious-pastry-food-sweets-factory-bread-chocolate-caramel-manufacturing-process-isolated-flat-vector-illustration_277904-13228](https://github.com/user-attachments/assets/d6fede54-d965-4129-929e-3406bc61593e)



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

![Screenshot 2024-12-10 180638](https://github.com/user-attachments/assets/a157c1f9-c319-490b-a6d9-78aa402ed7bd)
![Screenshot 2024-12-10 180821](https://github.com/user-attachments/assets/f25e9470-1d00-4475-8bba-0ca4ccfe464d)
![Screenshot 2024-12-10 180900](https://github.com/user-attachments/assets/96770598-42f2-4768-99a1-64608d8a38a8)


**[Click here to access the interactive dashboard](https://app.powerbi.com/view?r=eyJrIjoiN2YxZDQ5ZmItMTEwOC00ZDdkLWIxM2YtNjNhZjNmOWFlMGZkIiwidCI6ImY0M2MzMTgyLTcxZjAtNGRjOS04YjA0LTc0OTMwZTNmOGNkYSJ9)** 

## Key Insights

- **Sales Trends**: Revenue shows notable sales spikes in February, April, August, and November, while volume peaks occur in February and November.
- **Year-Over-Year (YoY) Metrics**: YoY sales reach €103 million with a growth rate of 107%, indicating significant market expansion.
- **Revenue by Categories**: Chips and snacks lead with 46% of revenue, followed by bakery products at 39%, candy at 11%, and chocolate and bars at 5%.
- **Top and Bottom Manufacturers**: 'Other' is the top manufacturer by revenue and volume, while 'Elite Sweets' ranks at the bottom.
- **Top-Selling Item**: 'Crusty Cheddar' emerges as the highest-selling item in terms of both revenue and volume.
- **Distribution Channels**: Small and specialty stores are the most profitable distribution channels, while supermarket stores are the least profitable.
- **Product Types**: Biscuits are the most popular product type, whereas candy is the least popular.
- **Packaging Type**: Bags are identified as the most popular packaging type.
- **Top Chocolate-Related Brands**: Silver Snacks and Cascade Mills.
- **Top Chips-Related Brands**: Land Corp and Fusion Snack.

## Recommendations

- **Expand Top-Selling Items**: Focus on increasing the production and marketing of high-performing products like 'Crusty Cheddar'.
- **Enhance Small Stores**: Invest in small and specialty stores which are the most profitable.
- **Improve Supermarket Sales**: Boost supermarket store sales through promotions and partnerships.
- **Innovate Packaging**: Continue to develop popular packaging types, especially bags.
- **Promote Biscuits**: Leverage the popularity of biscuits by introducing new flavors and varieties.
- **Revitalize Candy Category**: Develop new and exciting candy products to attract more consumers.
- **Target Marketing**: Utilize identified sales spikes for targeted seasonal marketing campaigns.
- **Optimize Brands**: Enhance the performance of top brands like Silver Snacks, Cascade Mills, Land Corp, and Fusion Snack.

## Tech Stack
Project relies on the following key technologies:

- `Power BI Desktop` Design, visualization, and interactive reporting.
- `DAX (Data Analysis Expressions)` Creation of calculations and measures supporting data visualizations.
- `Power Query` Clean and transform raw data into a structured format.
- 
## License
This project is licensed under the MIT License. You are free to use, modify, and distribute the code and visuals as long as the original license terms are maintained.

---

Enjoy exploring the Power BI Sales Insights and Forecasting Dashboard! If you have questions or feedback, feel free to contact me.

*Contact: ajaysonkatar@gmail.com*

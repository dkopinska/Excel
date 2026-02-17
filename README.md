# Project 1: 📊 Retail & Student Performance Analysis – Excel Project
📌 Project Overview

This project demonstrates practical Excel data analysis skills through two datasets:

Retail Sales Dataset – to analyse customer spending and product revenue

Student Performance Dataset – to assess student grades and subject performance

The project showcases structured tables, logical formulas, pivot tables, lookup functions, conditional formatting, and data visualisation to generate actionable insights.

🛍 Part 1: Retail Sales Data Analysis
🎯 Business Objective

Analyse retail transaction data to:

Identify high-value customer segments

Understand revenue drivers by product category

Compare spending patterns by demographic groups (gender, age, generation)

Support data-driven business decisions

📊 Analytical Approach

Structured Tables – Converted raw data into Excel Tables to enable:

Dynamic formula application

Improved readability

Scalable dataset management

Revenue Calculation – Calculated total revenue per transaction:

=[@Quantity]*[@[Price per Unit]]


Customer Segmentation by Age – Categorised customers for demographic insights:

=IF([@Age]<30,"Young Adult",IF([@Age]>=50,"Senior","Adult"))


Segments used to compare spending across different generations in pivot tables.

Pivot Tables – Analysed:

Compared total spending by gender
![alt text](https://github.com/user-attachments/assets/5fb30041-b34a-4713-9f05-7db7369bacc6)

Compared spending trends across age groups
![alt text](https://github.com/user-attachments/assets/63ee6aad-8dfb-4e62-bca7-68eb7b1b0306)


High-performing product categories

Category-Level Revenue Analysis – Used SUMIF to calculate revenue per product category:

=SUMIF($F$2:$F$1001,$L9,$J$2:$J$1001)


Transaction-Level Validation – Used VLOOKUP to retrieve and verify individual transaction totals:

=VLOOKUP(A8, retail_sales_dataset!$A$2:$J$1001, column_index, FALSE)

📈 Key Insights (Retail)

Senior customers had the highest average transaction value.

Beauty category generated the strongest revenue among female customers.

Young Adults showed higher purchase frequency but lower basket value.

These insights could inform targeted marketing campaigns and inventory planning.

🎓 Part 2: Student Performance Analysis
🎯 Business Objective

Analyse student grades to:

Identify top and bottom performers by subject

Calculate overall student performance averages

Highlight each student’s best and worst subject

Visualise performance for easy interpretation

📊 Analytical Approach

Conditional Formatting (Heatmaps) – Highlighted high and low performers.

Summary Statistics – Calculated:

=MAX(range)
=MIN(range)
=AVERAGE(B2:D2)


Best & Worst Subject per Student – Dynamically identified using:

=INDEX(B$1:D$1, MATCH(MAX(B2:D2), B2:D2, 0))  // Best subject
=INDEX(B$1:D$1, MATCH(MIN(B6:D6), B6:D6, 0))  // Worst subject


Data Visualisation – Bar charts to compare scores per student and per subject.
![alt text](https://github.com/user-attachments/assets/d609a0d6-f621-425a-9ba5-04a0d3a99642)

📈 Key Insights (Student Performance)

Students’ strongest subjects were identified at an individual level.

Overall average scores helped benchmark class performance.

Visualisations highlighted gaps and strengths across subjects.

🛠 Skills Demonstrated

Excel Tables & Structured References

Logical Formulas & Nested IF Statements

SUMIF & VLOOKUP / INDEX-MATCH

Pivot Tables & Demographic Analysis

Conditional Formatting (Heatmaps)

Sorting & Ranking

MAX, MIN, AVERAGE Functions

Data Visualisation (Bar Charts)

🔮 Potential Enhancements

Replace VLOOKUP with XLOOKUP for modern Excel

Build interactive dashboards with slicers and pivot charts

Automate reports with Power Query

Integrate KPI summary dashboards for real-time insights

🚀 Why This Project Matters

This project highlights your ability to:

Transform raw data into structured, analyzable formats

Apply logical formulas to segment and analyse data

Use pivot tables to generate business insights

Visualise results for decision-making

Communicate data-driven findings in a professional format




Project 2: Pivot Table Analysis Lab – Bike Sales Dataset (Data Questions)

📌 Project Overview

This project demonstrates the use of Excel Pivot Tables to analyse bike sales data across countries, markets, age groups, genders, and product categories. The analysis focuses on answering key business questions, identifying profitable segments, and deriving actionable insights.

The lab also serves as an exercise in data aggregation, segmentation, and insight generation using Excel Pivot Tables.

🎯 Business Objectives / Questions

Using the dataset, the following questions were addressed:

1. In which markets does Germany have customers?

2. What country has sales in all markets?

3. What are the most profitable markets by country, age group, and gender?

4. Any other findings?

Pivot Tables were used to systematically explore each question.

📊 Analytical Approach

Pivot Table Setup:

Rows: Country, Market, Age Group, Gender

Values: Sum of Revenue, Sum of Profit

Filters: Year = 2021, Month = December

Segmentation Analysis:

Age groups: Youth (<25), Young Adults (25–34), Adults (35–64), Seniors (64+)

Gender: Male, Female

📈 Key Insights

Geographic Insights:

1. Germany had customers in Hamburg, Hessen, and Nordrhein-Westfalen, primarily Adults (35–64).

No purchases were recorded from Young Adults or Seniors in December 2021.

![alt text](https://github.com/user-attachments/assets/7cde27eb-6a55-4792-8a0e-905e59580a99)


2. The United States had sales in all markets, followed by Australia.
   Other countries, such as France, Germany, and the UK, had sales in limited markets.
   
![alt text](https://github.com/user-attachments/assets/d3afed1e-8164-47ff-85f4-8bf8291a7334)


3. Profitable Segments:

 By Country:

Top 1: United States

Top 2: Australia

Top 3: France

The US and Australia together accounted for 67.7% of total revenue.

![alt text](https://github.com/user-attachments/assets/148f7bfe-82f5-4309-921f-1dce81972ad9)

By Age Group: Adults (35–64) contributed 57.2% of total profits; Young Adults (25–34) contributed 33%. Combined, these two segments made up 90.2% of profits.

By Gender: Female customers accounted for 59.6% of total sales, outperforming males.

![alt text](https://github.com/user-attachments/assets/44e6301f-dcc5-450e-abcd-b3ad40b77a6a)


4. Product-Level Insights:

Top-selling bike models in December 2021:

1.Mountain-200 Black (46)

2.Mountain-200 Black (38)

3.Mountain-200 Silver (38)

4.Mountain-200 Black (42)

5.Mountain-200 Silver (42)

These five Mountain-200 models accounted for 61% of total sales, highlighting strong short-term demand.

Gender-specific preferences:

Women: Mountain-200 Black, 46 → Mountain-200 Silver, 38 → Mountain-200 Silver, 42

Men: Mountain-200 Black, 38 → Mountain-200 Black, 42 → Mountain-400-W Silver, 46

Seasonal & Contextual Observations:

Low sales in Canada, Germany, and the UK may reflect harsh winter conditions.

Australia and certain US regions have milder winter climates.

Seasonality and month-specific trends should be analysed over multiple periods for strategic inventory planning.

🛠 Skills Demonstrated

Excel Pivot Tables for multi-dimensional analysis

Segmentation by age, gender, and market

Aggregation of sales revenue by country, market, and product

Product ranking and best-seller identification

Comparative analysis across demographic and geographic segments

Translating pivot table results into business insights

🔮 Recommendations for Business

Prioritise stock and promotions for Mountain-200 Black and Silver models

Target marketing campaigns toward Adults (35–64), particularly female customers

Consider seasonal trends in inventory planning

Extend analysis over multiple months to validate trends and forecast demand

🚀 Why This Project Matters

This lab demonstrates the ability to:

Transform raw transactional data into actionable insights

Apply Excel pivot tables for complex multi-level analysis

Segment customers and identify high-value markets

Link sales patterns to business strategy decisions

Communicate insights clearly for stakeholders and decision-makers


💡 Next Steps / Further Analysis

Analyse sales trends over multiple months to confirm seasonal insights

Explore correlation between marketing campaigns and sales

Build dynamic dashboards for real-time insights



# Project 3: Sales Analysis by County – Product Performance Dataset

📌 Project Overview

This project demonstrates Excel Pivot Table analysis and formula-based data categorisation on a product sales dataset for various counties in England. The analysis explores sales performance by county and product, and segments products based on sales volume, providing actionable insights for regional performance and inventory planning.

🎯 Business Objective

Analyse product sales across counties in England to:

Summarise sales performance by county and product

Categorise products based on sales volume (High, Medium, Low)

Identify top-performing counties and products

Provide insights to inform inventory, stocking, and regional marketing strategies

📊 Analytical Approach

Step 1: Pivot Table Analysis

Pivot tables were created with County in the rows and Products in the columns.

Sales Volume was used as the values to summarise total sales per product per county.

This allowed easy identification of which counties perform best for each product and overall sales patterns.

Step 2: Product Categorisation using SWITCH Function

Added a new column to categorise products based on sales volume:

=SWITCH(TRUE, C2 > 600, "High", C2 >= 300, "Medium", "Low")


Categories Defined:

High: Sales volume > 600

Medium: Sales volume between 300–600

Low: Sales volume < 300

Ensured all sales values were numerical and removed extra spaces.

Formula applied to all rows to quickly segment products by performance.

📈 Key Insights

County-Level Performance:

Cornwall: Highest total sales with Laptops (700) and Printers (400) performing strongly.

Essex: Strongest printer sales (800), indicating demand for office equipment in the region.

Yorkshire: High laptop sales (500) dominate the market, smartphones less in demand.

Lancashire & Greater Manchester: Balanced demand across laptops and smartphones.

Durham: Moderate performance across laptops and printers, but no high-volume sales.

Product Performance Segmentation:

High Sales: Printers in Essex (800), Laptops in Cornwall (700)

Medium Sales: Laptops in Yorkshire (500), Laptops in Lancashire (600), Smartphones in Greater Manchester (600)

Low Sales: Smartphones in Lancashire (150), Smartphones in Yorkshire (200), Laptops in Durham (250)

Overall Observations:

Laptops consistently show strong sales across multiple counties.

Printers show peak sales in specific counties, highlighting regional demand.

Smartphones are generally lower-performing compared to laptops and printers, except in Greater Manchester.

🛠 Skills Demonstrated

Excel Pivot Tables for multi-dimensional summarisation

Formula-based data categorisation using SWITCH

Aggregation and comparison of sales across counties and products

Identifying high-performing counties and products for inventory and marketing decisions

Clean, structured approach to data preparation and analysis

🔮 Recommendations for Business

Focus inventory and promotions on Laptops and Printers in high-performing counties.

Monitor low-sales counties for potential marketing campaigns or adjustments in product mix.

Extend analysis over multiple months or products to identify seasonal trends and demand cycles.

Use the sales categorisation framework (High/Medium/Low) for dynamic reporting dashboards.


⚡ Potential Improvements & Next Steps

Time Series Analysis: Extend analysis over multiple months or years to detect seasonal trends and forecast future demand by county.

Granular Segmentation: Segment sales by additional dimensions, e.g., customer demographics, product category, or price range, for more targeted insights.

Advanced Formulas & Automation: Use dynamic formulas or Excel’s Power Query / Power Pivot to automate categorisation and reporting.

Data Visualisation: Create interactive dashboards with charts, heatmaps, or slicers to make county and product performance more visually intuitive.

Scenario Planning: Model potential inventory or marketing strategies based on predicted high/low sales counties to optimise stock and promotional campaigns.



# Project 4: Bike Sales Visualisations Lab – Trends, Revenue & Demographics

📌 Project Overview

This project demonstrates Excel chart-based analysis on bike sales data. Using line, bar, and pie charts, the lab explores:

Trends in annual revenue and profit over time

Revenue contributions by product category across countries

Revenue distribution by customer age groups

The goal is to derive actionable business insights for sales planning, marketing, and inventory management.

🎯 Business Objective

Analyse bike sales to:

Visualise annual profit and revenue trends (2017–2021)

Compare revenue contributions by product category (Accessories, Bikes, Clothing) across countries

Understand customer revenue distribution by age group

Identify high-performing countries, product categories, and customer segments

Provide insights for strategic sales, marketing, and inventory decisions

📊 Analytical Approach

Step 1: Line Chart – Annual Trends

Created a line chart showing Annual Profit and Annual Revenue from 2017–2021.

Observed growth trends, peaks, and year-over-year changes.

Step 2: Bar Chart – Revenue by Product Category & Country

Created a stacked bar chart summarising total revenue by product category per country.

Visual comparison highlights which product categories dominate revenue in each country.

Step 3: Pie Chart – Revenue by Age Group

Created a pie chart showing revenue distribution across customer age groups.

Categorised age groups: Youth (<25), Young Adults (25–34), Adults (35–64), Seniors (64+).

Visualisation helps identify which age segments contribute most to overall revenue.

📈 Insights from Visualisations

Line Chart – Annual Trends:

![alt text](https://github.com/user-attachments/assets/603bad55-4d4b-4f2e-be95-313a6874bae4)


Revenue and profit increase steadily from 2017–2021.

Profit growth slightly outpaces revenue, indicating improved margins.

Bar Chart – Revenue by Product Category & Country:

![alt text](https://github.com/user-attachments/assets/8ff63225-4421-4744-a878-4f0db5ced47a)

Bikes dominate revenue, particularly in the US and Australia.

Accessories and Clothing contribute moderately; opportunities exist for upselling.

US and Australia are key markets, together contributing over 57% of total revenue.

Pie Chart – Revenue by Age Group:

![alt text](https://github.com/user-attachments/assets/99355353-101e-479d-b9f0-5a8d1b13e5dc)


Adults (35–64) are the largest revenue contributors (~50%).

Young Adults (25–34) contribute ~36%, indicating a strong secondary segment.

Youth (<25) represent 14% of revenue; Seniors (<1%) contribute minimally.

Insights suggest marketing campaigns should prioritise Adults and Young Adults.

🛠 Skills Demonstrated

Excel line, bar, and pie chart creation for multi-dimensional analysis

Visualising temporal trends, geographic patterns, and customer segments

Comparative analysis across products, countries, and age groups

Identifying high-value markets, products, and customer segments

Translating visual data into business insights

🔮 Potential Improvements & Next Steps

Segmented Analysis: Combine age groups with gender and country to identify high-value demographic segments.

Time-Series Forecasting: Extend trends analysis to forecast future revenue and profit.

Profit Margin Analysis: Incorporate cost data to evaluate profitability per product category and country.

Interactive Dashboards: Build dynamic Excel dashboards with slicers for product, country, and age group.

Seasonal/Monthly Analysis: Examine month-by-month sales patterns for inventory and marketing optimisation.

🚀 Why This Project Matters

This lab demonstrates the ability to:

Transform raw sales data into actionable insights

Track revenue and profit trends over time

Identify high-value products, regions, and customer segments

Communicate insights clearly for business stakeholders







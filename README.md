### CoffeeShop-Dashboard
<img src="https://github.com/nsankareswari-70/CoffeeShop-Dashboard/blob/e2adf22103773699cd8cc4bd5d5432b15bdcfb42/coffeeshop.png" height=300 width = 300 alt="Description" class="center">
Project Overview:

To better understand customer purchase behavior and streamline operational efficiency, I collected transactional data from January to June 2023. The primary goal of this project is to transform the raw dataset into an interactive, dynamic dashboard that franchise owners can use to identify key patterns, trends, and opportunities for business growth.

Core Objectives

Profile and Prepare the Raw Data for Analysis
Conduct data cleaning, validation, and preprocessing to ensure accuracy and usability. This includes handling missing values, standardizing formats, and structuring the dataset for meaningful analysis.

Explore the Data Using Excel Pivot Tables
Perform exploratory data analysis (EDA) to summarize sales performance, customer behavior, and product trends. Pivot tables are used to reveal relationships, identify anomalies, and establish the foundation for deeper insights.

Build a Dynamic Dashboard to Visualize Key Patterns and Trends
Develop a user-friendly, interactive dashboard that enables franchise owners to filter, drill down, and visualize sales trends, purchasing patterns, and operational insights to support data-driven decision making.

### PREPARING THE DATA FOR ANALYSIS
- Getting familiarize with the data. How many transactions were recorded. Over what period of time? What products and product categories were sold?
- Adding a new column to calculate Revenue(price*quantity)
- Adding new columns to calculate Month and Dayofweek based on the transaction date( In addition to that display them as text - January,February.. and for days Sun,Mon,Tue ..)
- Adding a new column to extract Hour from the transaction time.
Results:
- How many transactions were recorded?
149456
- Over what period of time?
1/1/2023 - 6/30/2023
- What products and product categories were sold?
  Product categories:
9 categories - 1.Bakery, 2.Branded 3. Coffee 4. Coffee beans 5. Drinking Chocolate
6.Flavours 7.Loose Tea 8.Packaged Chocolate 9.Tea

  By applying Filter for the table columns we can see the available products from the Product type column.
  Create a new column for Revenue to multiply price*quantity and make it as currency format with two decimal places.
  From the Transaction Date,Transaction time columns we can create new columns by using power query or by simply using excel functions like month(),day(),dayofweek(),hour() and text() functions.

### EXPLORING THE DATA WITH PIVOT TABLES
- Inserting a PivotTable on a new tab to show revenue by month
- Adding two more PivotTables (on the same sheet) to show the number of transactions by day of week and hour of day.
- Adding a PivotTable (on the same sheet) to show the number of transactions by product category, sorted descending by transactions.
- Adding a PivotTable (on the same sheet) to show the number of transactions and revenue by product type, sorted descending and filtered to the Top 15 (by transactions)
<img src="https://github.com/nsankareswari-70/CoffeeShop-Dashboard/blob/1ffece6851071d2de403372ce27fa9ceec105af0/cshop1.png">

### BUILDING A DYNAMIC DASHBOARD
- Adding Pivot Charts to show revenue by month as a line chart, transactions by day of week and hour of day as column charts and transactions by product category as a bar chart.
- Assembling the charts into a rough dashboard layout, and include space for the PivotTable showing Top 15 product types.
- Adding a slicer for store location and connect it to all of the PivotTables on the sheet
- Adjusting formats, alignments and polishing to finalize the dashboard (like removing unwanted buttons and gridlines from the chart)
<img src="https://github.com/nsankareswari-70/CoffeeShop-Dashboard/blob/67932be4e47e0074079d88d29278e11dab1b0f29/cshop2.png">

Data Driven Insights:
From the above Hour of Day chart for Lower Manhattan location after 6pm - Number of transactions is very low.So maybe we are losing money by keeping store open past 6 o'clock and can improve our margin by changing the operating hours.
Barista Espresso seems to be the popular product in this area.Coffee and Tea are the next best selling products.



  

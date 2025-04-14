Task 2 – Data Visualization and Storytelling

Tool: Tableau Public
Dataset: Sample Superstore (Kaggle)

Objective
To analyze sales and profit trends using calculated fields and create 5 effective, insight-driven charts with proper titles, contexts, and storytelling.

Calculated Fields Used

1. Profit Ratio:
SUM([Profit]) / SUM([Sales])
→ Used to measure profitability.


2. Profit Status:

IF [Profit Ratio] < 0 THEN "LOSS"
ELSE "PROFITABLE"
END

→ Identifies profitable vs loss-making records.


3. Sales Category:

IF [Sales] > 150000 THEN "HIGH"
ELSE "MEDIUM"
END

→ Categorizes sales volume.


4. % of Total Orders:
COUNT([Order ID]) / TOTAL(COUNT([Order ID]))
→ Used in pie chart to show order distribution.

Charts Created (5)

1. Profit Ratio by Category

Title: Technology Has the Highest Profit Margins – Furniture Lags Behind

Type: Bar chart

Insight: Technology performs best; Furniture lowest.

Field: Profit Ratio


2. Sheet2 – Sales vs Profit

Title: High Sales Product Aren’t Always Profitable – See Red Zones

Type: Scatter Plot

Field: Profit Status, Sales, Profit



3. Sheet3 – Order Distribution

Title: Consistent Sales Growth but Profit Success
Type: Pie Chart
Field: Sales Category, % of Total Orders


4. Sales Category Pie Chart

Title: Most Orders Fall in the Medium Sales Category

Type: Pie chart

Insight: 98% orders are medium-sized.

Field: Sales Category, % of Total Orders



5. Profitability by Region

Title: West Region is Most Profitable – Central Struggles

Type: Bar chart

Insight: Central is loss-making; West leads.

Field: Profit Ratio, Profit Status

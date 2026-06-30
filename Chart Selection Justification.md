# Chart Selection Justification

## Overview
The dashboard was designed following visualization best practices to ensure clear communication of business insights. Appropriate chart types were selected based on the nature of the data and the business questions.

---

## 1. Sales Trend View – Line Chart

**Business Question:** How are sales changing over time?

**Justification:**
A line chart is the most suitable visualization for time-series data as it clearly shows trends, patterns, seasonality, and fluctuations in sales over time.

---

## 2. Regional Performance – Map

**Business Question:** Which regions perform best?

**Justification:**
A map visualization effectively displays geographical sales distribution and enables quick identification of high-performing and low-performing regions.

---

## 3. Category Profitability – Treemap

**Business Question:** Which categories and sub-categories contribute most to profit?

**Justification:**
A treemap efficiently represents hierarchical data and allows comparison of category contributions using both size and color. Large blocks indicate higher sales, while color indicates profitability.

---

## 4. Customer Segment Analysis – Bar Chart

**Business Question:** Which customer segment generates the highest sales?

**Justification:**
Bar charts provide easy comparison between discrete categories and clearly highlight differences in sales performance among customer segments.

---

## 5. Shipping Performance – Stacked Bar Chart

**Business Question:** Which shipping modes experience delays?

**Justification:**
A stacked bar chart compares shipping modes while simultaneously showing the distribution of delivery delay categories, making operational performance easier to evaluate.

---

## 6. Discount vs Profit Analysis – Scatter Plot

**Business Question:** How does discount affect profit?

**Justification:**
Scatter plots are ideal for analyzing relationships between two continuous variables. The visualization helps identify correlations, trends, and outliers between discount levels and profit.

---

## 7. Return Analysis – Highlight Table

**Business Question:** Which regions and customer segments have higher return rates?

**Justification:**
A highlight table uses color intensity to quickly identify areas with high return rates, making comparison across regions and customer segments straightforward.

---

# Visualization Design Principles Applied

## Correct Chart Selection
Each chart type was selected based on the underlying business question and data characteristics.

## Clear Hierarchy
Key performance indicators (KPIs) such as Total Sales, Total Profit, and Profit Margin are positioned at the top of the dashboard to provide immediate business context.

## Minimal Clutter
Unnecessary gridlines, excessive labels, and redundant legends were removed to improve readability.

## Consistent Color Usage
Consistent colors were used throughout the dashboard:
- Blue shades for sales metrics
- Green shades for positive performance
- Red shades for losses or delays

## Proper Labels
All charts include meaningful titles, axis labels, and data labels where necessary.

## Readable Titles
Chart titles clearly describe the business question addressed by each visualization.

## Appropriate Sorting
Bar charts are sorted in descending order to facilitate quick comparison.

## Useful Filters
Interactive filters such as Region, Category, Customer Segment, Ship Mode, and Order Date were added to allow users to explore data dynamically.

## Avoidance of Misleading Scales
Default axis scales were maintained, and truncated axes were avoided to ensure accurate interpretation.

## Focus on Business Interpretation
The dashboard emphasizes actionable business insights related to sales performance, profitability, customer behavior, shipping efficiency, and return patterns.


#TASK 10
# Chart Selection Justification

## 1. Sales Trend View

### Business Question
How are sales changing over time?

### Chart Type
Line Chart

### Why This Chart Is Appropriate
A line chart is ideal for time-series analysis because it clearly displays trends, fluctuations, and seasonality in sales over time.

### Fields Used
- Columns: Order Date (Month)
- Rows: Sales
- Filter: Region, Category, Customer Segment, Order Date

### Design Principle Applied
Time-based data is represented using a continuous axis to ensure accurate trend interpretation.

### Mistake Avoided
Avoided using pie charts or bar charts for time-series data, which would make trends difficult to identify.

---

## 2. Regional Performance

### Business Question
Which regions contribute the highest sales and profit?

### Chart Type
Map

### Why This Chart Is Appropriate
A map effectively visualizes geographical performance and helps identify high-performing and low-performing regions.

### Fields Used
- Geographic Field: State
- Color: Profit
- Label: Sales
- Filter: Region, Category, Date

### Design Principle Applied
Geographical data is displayed spatially to improve business understanding.

### Mistake Avoided
Avoided using multiple bar charts for geographical analysis, which would reduce spatial context.

---

## 3. Category Profitability View

### Business Question
Which categories and sub-categories contribute most to profitability?

### Chart Type
Treemap

### Why This Chart Is Appropriate
Treemaps efficiently display hierarchical relationships while simultaneously comparing contribution and profitability.

### Fields Used
- Label: Sub-Category
- Size: Sales
- Color: Profit

### Design Principle Applied
Both color and size are used to represent different business metrics without overcrowding the visualization.

### Mistake Avoided
Avoided using excessive bar charts, which would make the dashboard repetitive.

---

## 4. Customer Segment Analysis

### Business Question
Which customer segment generates the highest sales?

### Chart Type
Bar Chart

### Why This Chart Is Appropriate
Bar charts provide clear comparison among discrete categories and allow quick identification of top-performing customer segments.

### Fields Used
- Columns: Customer Segment
- Rows: Sales
- Label: Sales
- Color: Customer Segment

### Design Principle Applied
Categories are compared using a common baseline for accurate interpretation.

### Mistake Avoided
Avoided pie charts because differences between segments would be harder to compare.

---

## 5. Shipping Performance

### Business Question
Which shipping modes experience delays?

### Chart Type
Stacked Bar Chart

### Why This Chart Is Appropriate
Stacked bars enable comparison of shipping modes while showing the distribution of delivery delay categories.

### Fields Used
- Rows: Ship Mode
- Columns: Number of Orders
- Color: Shipping Delay Bucket

### Design Principle Applied
Color coding highlights delivery performance categories clearly.

### Mistake Avoided
Avoided using line charts because shipping modes are categorical rather than time-based.

---

## 6. Discount vs Profit Analysis

### Business Question
How does discount impact profitability?

### Chart Type
Scatter Plot

### Why This Chart Is Appropriate
Scatter plots are best suited for analyzing relationships between two continuous variables and identifying correlations or outliers.

### Fields Used
- Columns: Discount
- Rows: Profit
- Color: Category
- Detail: Product Name

### Design Principle Applied
Individual observations are displayed to reveal patterns and anomalies.

### Mistake Avoided
Avoided using bar charts because they cannot effectively represent relationships between continuous variables.

---

## 7. Return Analysis

### Business Question
Which region and customer segment combinations have the highest return rates?

### Chart Type
Highlight Table

### Why This Chart Is Appropriate
Highlight tables enable quick identification of high and low return rates using color intensity.

### Fields Used
- Rows: Region
- Columns: Customer Segment
- Color: Return Rate
- Label: Return Rate

### Design Principle Applied
Color intensity draws attention to areas requiring immediate business action.

### Mistake Avoided
Avoided overcrowded tables with excessive numerical values, improving readability.

---

# Dashboard-Level Design Decisions

## Filters Added
- Region
- Category
- Customer Segment
- Ship Mode
- Order Date

## Interactive Feature
Selecting a region on the map filters the remaining dashboard views, enabling detailed exploration.

## Consistent Color Usage
- Green: Positive performance/high profit
- Red: Negative performance/loss/delay
- Blue: Neutral metrics and sales comparisons

## Clutter Reduction
Unnecessary gridlines, redundant legends, and excessive labels were removed to improve readability.
# Amazon Sales Analysis – SQL Capstone Project

# Project Overview:
This project focuses on analyzing Amazon sales data using MySQL to extract meaningful business insights. The analysis helps understand product performance, sales trends, and customer behavior, enabling data-driven decision-making.

The project follows a structured data analytics approach including: data wrangling, 
feature engineering, and 
advanced SQL querying.

---

# Objectives:
- Identify best and worst performing product lines.
- Analyze sales trends across time.
- Understand customer segments and profitability.
- Perform feature engineering for better insights.
- Strengthen SQL querying and analytical skills.

---

# Dataset Description:
The dataset contains transactional sales data with attributes such as:
- Invoice ID  
- Branch  
- City  
- Customer Type  
- Gender  
- Product Line  
- Unit Price  
- Quantity  
- Tax  
- Total  
- Date  
- Time  
- Payment Method  
- Rating  

---

# Tools & Technologies:
- MySQL
- DBMS / SQL Workbench
- Git & GitHub

---

# Data Wrangling:
- Created database and tables
- Applied **NOT NULL constraints** to ensure data quality
- Verified data consistency and integrity

---

# Feature Engineering:
Additional columns were created to enhance analysis:
- timeofday → Morning / Afternoon / Evening  
- dayname → Day of the week  
- monthname → Month of the year  

These features help in identifying time-based sales patterns.

---

# Analysis Performed:

1. Product Analysis
- Most selling product lines
- Product lines generating highest revenue
- Product lines needing improvement

2. Sales Analysis
- Sales trends by month and day
- Revenue distribution across branches and cities
- Time-of-day sales performance

3. Customer Analysis
- Customer segmentation (Member vs Normal)
- Gender-based purchasing behavior
- Most profitable customer groups
- Payment method preferences

---
# Insights:

1. product lines like food and beverages consistently outperform    others and underperforming is health and beauty

2. Sales peak during specific times of the day i.e. afternoon

3. Members contribute higher average revenue

4. Customer purchasing behavior varies by gender and city
---
# Future Enhancements:

1. Integrate with Power BI / Tableau dashboards

2. Automate reports

3. Apply advanced analytics and forecasting

---
# conclusion:
This capstone project demonstrates strong SQL skills, structured analytical thinking, and real-world business insight generation using data.

---

# Sample SQL Queries:
```sql
-- Most selling product line
SELECT `product line`, SUM(quantity) AS total_sold
FROM amazon
GROUP BY `product line`
ORDER BY total_sold DESC;



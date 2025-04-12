# Vrindra-Store-Analysis-Using-Excel
Vrinda Store Data Analysis
This project showcases a beginner-level yet professional-looking dashboard made in Microsoft Excel, focusing on retail data analytics. The goal was to clean the data, process it, and generate meaningful visual insights using pivot tables and charts.

Step 1: Data Cleaning
Opened the Excel dataset and checked for null or missing values.

Removed all blank rows or entries manually or via Excel filters.

Ensured all data types were correct:

Dates recognized as Date.

Text fields like Gender or State as Text.

Numeric fields like Amount formatted as Number.

Step 2: Data Processing
Age Categorization:
Created a new column to group age values into:

Teenagers: Ages 13–19

Adults: Ages 20–59

Seniors: Age 60+

Used the IF formula in Excel for this:

excel
Copy
Edit
=IF(Age<20,"Teenager",IF(Age<60,"Adult","Senior"))
Month Extraction:
From the Date column, extracted Month Names using:

excel
Copy
Edit
=TEXT(Date, "mmmm")
This new Month column helped in time-based trend analysis.

📈 Step 3: Data Analysis & Dashboard Creation
1. 📊 Orders vs Sales Over Time
Created a Pivot Table with:

Month in Rows

Amount (Sum) and Order ID (Count) in Values

Used a Combo Chart:

Column chart for Order Count

Line chart for Total Sales

Placed Order Count on a secondary axis for balance

Chart Formatting:

Disabled gridlines and field buttons

Axis label formatted to Millions (M) via:

mathematica
Copy
Edit
Axis → Format → Number Format → 0.00,,"M"
2. 🧑‍🤝‍🧑 Gender-Based Spending
Created a Pivot Table:

Gender in Rows

Amount in Values (Sum)

Used a Pie Chart to visualize:

Removed legend

Enabled data labels with percentages

Customized label placement and removed fills/outlines for a clean look

3. 🛍️ Order Status Breakdown
Similar setup to the gender pie chart:

Order Status in Rows

Order ID in Values (Count)

Built a Pie Chart showing proportion of statuses like Delivered, Pending, etc.

Applied same formatting: no legend, custom label placements.

4. 🌐 Order Channels
Built a Pivot Table:

Order Channel in Rows (like Online, In-Store)

Order ID in Values (Count)

Inserted a Pie Chart to visualize share of each order channel.

Removed clutter:

Removed legends

Added data labels with percentages

Dragged labels inside slices and removed fill/outline

5. 🗺️ Top States by Order Count
Pivot Table:

State in Rows

Order ID in Values (Count)

Sorted values from largest to smallest

Inserted a Bar Chart (horizontal column chart)

This chart clearly showed which states had the most orders

6. 🧓📊 Age and Gender Analysis
Created a combined Pivot Table:

Age Category and Gender in Rows

Order ID or Amount in Values

Inserted a Clustered Column Chart to compare groups

Helped identify which gender in which age group was most active in shopping

📁 Files Included
Vrinda Store Data Analysis.xlsx: Full Excel workbook with data, pivot tables, and dashboard

Store Data analytics Project.txt: Rough documentation notes used as a draft

(Optional) Dashboard Screenshot.png: Add this manually if you want a visual preview in your GitHub

🚀 Key Learnings
How to clean and categorize Excel data manually

Creating useful Pivot Tables

Building insightful and aesthetic Dashboards

Using Combo Charts, Pie Charts, and Bar Charts effectively

Turning raw data into business insights

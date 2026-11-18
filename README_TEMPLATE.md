# PM-06-PS02: SmartStore Python and SQL Assignment

# Project Overview

This project involves analysing fictional retail data for SmartStore, a retail business operating across multiple branches.

The objective is to demonstrate how Python programming, mathematical principles, algorithms, SQL and database technologies can be used to analyse retail data, solve business problems and support management decision-making.

The project focuses on branch performance, product revenue, customer purchasing behaviour, stock availability and order prioritisation.

# Practical Activities (PA)

# PA0201 – Conduct Basic Programming
Demonstrated fundamental Python programming concepts, including:
- Variables and data types.
- Lists, dictionaries, tuples and sets.
- Conditional statements (if, elif and else).
- For loops and while loops.
- Functions and return statements.
- User inputs and outputs.
- Error handling using try and except.
- Code comments and logical program execution.

# PA0202 – Apply Basic Mathematical Principles and Methods
Applied mathematical calculations to solve retail business problems, including:
- Total revenue and total cost.
- Gross profit and gross profit percentage.
- Profit per unit.
- Average order value.
- Minimum and maximum order values.
- Branch revenue contribution.
- Discounts and VAT calculations.
- Product stock value.
- Customer purchase frequency.

# PA0203 – Use Algorithms
Developed and implemented a business algorithm to classify orders according to their processing priority.

The project included:
- Writing pseudocode before implementation.
- Applying sequence, selection and repetition.
- Using conditional statements to classify orders.
- Searching and sorting information.
- Testing the algorithm using different scenarios.
- Comparing expected and actual results.

# PA0204 – Work with Software Packages
Used Python, pandas, Jupyter Notebook and SQLite to process and analyse retail information.

Activities included:
- Connecting Python to an SQLite database.
- Creating and working with database tables.
- Writing SQL queries.
- Filtering, sorting and grouping records.
- Using aggregate functions.
- Joining related database tables.
- Loading SQL query results into pandas DataFrames.
- Performing additional calculations using Python.
- Exporting analysis results into CSV reports.

# Tools Used

| Tool | Purpose |
|---|---|
| Python | Programming, calculations and algorithms |
| pandas | Data manipulation and analysis |
| Jupyter Notebook | Writing, executing and documenting code |
| SQLite | Relational database management |
| SQL | Retrieving, filtering and analysing database information |
| GitHub | Version control and project submission |
| Loom | Recording the project demonstration |

# Database Tables

The project uses six main database tables:

# 1. Branches
Contains information about SmartStore's different retail branches. It is used to identify branch locations and analyse revenue performance.

# 2. Products
Contains product information, including product names, categories, selling prices and costs. It supports product revenue and profitability analysis.

# 3. Customers
Contains customer information used to analyse customer types, purchasing behaviour and spending patterns.

# 4. Orders
Contains customer order information, including order identifiers, branch information, order totals and order statuses.

# 5. Order Items
Contains individual products included in each order, including quantities and selling prices. It helps calculate product-level sales revenue.

# 6. Stock
Contains product stock information across different branches. It is used to identify low-stock products and support inventory management.

# Python Activities

The following Python programming concepts were demonstrated:

- Creating variables and working with different data types.
- Using lists and dictionaries to organise information.
- Applying conditional statements to make decisions.
- Using loops to process multiple records.
- Creating reusable functions for calculations.
- Handling invalid inputs and basic programming errors.
- Using pandas to load and manipulate CSV datasets.
- Creating DataFrames and analysing retail information.
- Connecting Python to SQLite databases.
- Exporting processed information into CSV files.

# Mathematical Methods

The following mathematical calculations were applied:

| Calculation | Purpose |
|---|---|
| Revenue = Selling Price × Quantity Sold | Calculates sales revenue |
| Total Cost = Cost Price × Quantity Sold | Calculates product costs |
| Gross Profit = Revenue − Total Cost | Measures profit before operating expenses |
| Gross Margin = (Gross Profit ÷ Revenue) × 100 | Measures profitability as a percentage of revenue |
| Average Order Value = Total Revenue ÷ Number of Orders | Measures average customer order value |
| Branch Contribution = (Branch Revenue ÷ Total Revenue) × 100 | Measures each branch's revenue contribution |
| Discount = Original Price × Discount Rate | Calculates price reductions |
| VAT = Taxable Amount × VAT Rate | Calculates VAT |
| Stock Value = Quantity in Stock × Unit Cost | Measures inventory value |

These calculations demonstrate how mathematical principles can support financial analysis, profitability measurement and retail management decisions.

# Algorithm – Order Priority Classification

A simple order-priority algorithm was developed to help SmartStore determine which orders should receive attention first.

The algorithm considers:
- Order status.
- Stock availability.
- Delivery urgency.
- Order value.

# Business Rules

| Condition | Priority |
|---|---|
| Order is cancelled | Do Not Process |
| Stock is unavailable | Stock Hold |
| Urgent delivery and order value is R3,000 or more | High Priority |
| Urgent delivery | Medium Priority |
| Order value is R3,000 or more | Medium Priority |
| All other valid orders | Standard Priority |

The algorithm was implemented in Python using conditional statements and tested with different input scenarios to verify that the expected classifications were returned.

# SQL Queries

SQL was used to retrieve and analyse information from the SmartStore relational database.

The main SQL skills demonstrated included:

- SELECT – retrieving database records.
- WHERE – filtering information.
- ORDER BY – sorting query results.
- GROUP BY – grouping records.
- HAVING – filtering aggregated results.
- COUNT, SUM, AVG, MIN and MAX – performing calculations.
- INNER JOIN – combining related tables.
- CASE – implementing conditional classifications.
- LIMIT – restricting the number of returned records.

# Main Business Questions Answered

1. Which branch generated the highest completed revenue?
2. Which ten products generated the highest completed sales revenue?
3. Which customers spent the most?
4. Which products were at or below their reorder levels in each branch?
5. What were the completed revenue and gross profit figures by product category?

# Key Findings

The analysis was designed to identify important business insights relating to SmartStore's retail performance.

The key findings from the completed analysis include:

1. Branch Performance:** [Insert the name of the branch with the highest completed revenue and its revenue.]

2. Product Performance:** [Insert the top-performing product and its completed sales revenue.]

3. Customer Spending:** [Identify the highest-spending customer and their total completed purchases.]

4. Stock Management:** [Summarise the number of low-stock products and the branches requiring replenishment.]

5. Category Profitability:** [Identify the category generating the highest gross profit.]

# Management Recommendations

- Prioritise stock replenishment for products below their reorder levels.
- Monitor branch revenue to identify strong and underperforming locations.
- Use customer spending patterns to develop customer retention strategies.
- Prioritise products and categories that generate strong revenue and gross profit.
- Use order-priority classifications to improve order processing and fulfilment.

# Project Outputs

The project produces the following reports:

- Branch performance report.
- Product performance report.
- Prioritised orders report.
- Low-stock report.

The reports are exported in CSV format and stored in the outputs folder.

# How to Run the Project

1. Download or clone this GitHub repository.
2. Extract the project files if downloaded as a ZIP archive.
3. Ensure all required datasets and the SQLite database are available in the data folder.
4. Install Python and the required libraries.
5. Open the project folder in VS Code or Jupyter Notebook.
6. Open `PM06_PS02_Python_SQL_Guided_Assignment.ipynb`.
7. Run the notebook cells sequentially from top to bottom.
8. Review the displayed results and generated reports.

# Required Python Libraries

```python
pip install pandas numpy matplotlib
```

SQLite is accessed through Python's built-in `sqlite3` library.

# Project Structure

```text
PM-06-PS02-SmartStore/
│
├── data/
│   ├── customers.csv
│   ├── products.csv
│   ├── branches.csv
│   ├── orders.csv
│   ├── order_items.csv
│   ├── stock.csv
│   └── smartstore.db
│
├── outputs/
│   ├── branch_performance.csv
│   ├── product_performance.csv
│   ├── prioritised_orders.csv
│   └── low_stock_report.csv
│
├── PM06_PS02_Python_SQL_Guided_Assignment.ipynb
├── smartstore_queries_starter.sql
└── README.md
```

# Conclusion

This project demonstrates how Python programming, mathematical principles, algorithms and SQL can be combined to analyse business data and solve practical retail problems.

It provides practical experience in data processing, database management, financial calculations, algorithm development and business reporting.

The project also demonstrates the importance of using data-driven insights to support operational and management decisions.

# Author

Name: Peter Mavazhe

Qualification: QCTO Occupational Certificate – Data Science Practitioner

Institution: Zaio Institute of Technology

Project: PM-06-PS02 – Python and SQL Assignment


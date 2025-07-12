# amazon-product-review
Exploratory Data Analysis on Amazon product reviews, including sales, ratings, discounts, and product insights using  pivot tables and Excel.

STEP-BY-STEP IN EXCEL & PIVOT:
Step 1: Load and Clean the Data
Open Excel, import the dataset (CSV/XLSX).

Check for:
Missing values

Inconsistent data types (e.g., price as text)

Comma-separated lists (e.g., reviews or ratings may need to be parsed)

Create new columns:
Discount % = (Actual Price - Discounted Price) / Actual Price

Revenue Estimate = Rating Count × Discounted Price (or Actual)

Step 2: Use Pivot Tables to Answer Questions
Use Excel's PivotTable for each question:

1. Average discount % by category
Rows: Category
Values: Avg of Discount %
2. Number of products per category
Rows: Category
Values: Count of Product Name
3. Total reviews per category
Values: Sum of Review Count
4. Top-rated products
Sort by Rating (descending)
5. Actual vs Discounted Price by Category
Rows: Category
Values: Avg of Actual Price, Avg of Discounted Price
6. Most-reviewed products
Sort by Review Count
7. Products with ≥ 50% discount
Apply filter: Discount % ≥ 50%
Count rows
8. Rating distribution
Group ratings (3.0, 3.5, etc.)
Count of products per rating
9. Total potential revenue by category
Revenue = Actual Price * Rating Count
10. Product count by price range
Create a bucket column:
 IF(price < ₹200, "<200", IF(price ≤ ₹500, "200–500", ">500"))
11. Discount vs Rating
Use a scatter plot or correlation function
12. Products with < 1,000 reviews
Apply filter and count
13. Categories with highest discount products
Sort Discount column within each category
14. Top 5 products: Rating + Review combo
Create a score column (Rating × log(Reviews)) and sort

Final Task: Create an Excel Dashboard

Use:
Pivot Charts

Slicers (by category or rating)

KPIs (Avg rating, total reviews, revenue, etc.)

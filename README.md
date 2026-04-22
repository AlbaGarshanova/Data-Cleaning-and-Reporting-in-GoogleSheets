1. Overview
The task was to clean and prepare data for analysis.
The goal was to check data quality and fix issues to make datasets ready for use.

2. Datasets
Transactions (20,000 records, 2017)
Customer (4,000 customers)
NewCustomerList (1,000 customers)
CustomerAddress (3,999 records)

3. Key Findings
Transactions
No duplicates found
2% missing online_order→ filled as "blank"
1% missing product data → removed
Missing quantity column
Unclear column: product_first_sold_date
Customers
Inconsistent gender values → standardized to Famel/Male/Unspecified
Missing data:
job_title (497)
job_industry_category (656)
last_name (125)
87 missing DOB + 1 incorrect value
default column is not usable
Address
Inconsistent state format → standardized (NSW, QLD, etc.)
Missing customer IDs after merge
Unclear column: property_valuation
NewCustomerList
No customer_id (no primary key)
17 missing DOB
5 unnamed columns without description

4. Cleaning Actions
Removed incorrect and incomplete records
Replaced missing categorical values with "unspecified"
Standardized text fields (gender, state)
Fixed data types (dates, numbers)
Used basic validation and formatting in Google Sheets

5. Recommendations
Add primary keys to all tables
Define clear data structure and column descriptions
Use data validation (dropdowns, formats)
Avoid missing critical fields (e.g., quantity, IDs)

7. Conclusion
The data required cleaning but is now more consistent and ready for analysis.
After improvements, it can be used for reliable business insights.


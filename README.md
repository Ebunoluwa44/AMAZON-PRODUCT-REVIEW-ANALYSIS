# AMAZON-PRODUCT-REVIEW-ANALYSIS
### This project analyses Amazon Product reviews using excel to identify key trends, product performance , customer sentiment, etc.
## Key Features 
- Data cleaning (duplicates, missing values)
- Review aggregation by product
- Summary statistics and visualizations.
## Data Cleanaing Actions:
- Product name shortening to reduce long product names for cleaner charts
#### =TRIM(LEFT(B2,FIND(" ",B2,FIND(" ",B2,FIND(" ",B2)+1)+1)))
- Removes Duplicate
- Delete unneccessarry columns (those that are not relevant to the analysis)
- About Product shortening fuction:
#### =TRIM(LEFT(I2,FIND(".",I2&".")+0))
## ANALYSIS (PIVOT TBLES)
### Average discount % by category
- Rows: Category
- Values: Average of discount %
### Products per category
- Rows: Category
- Values: count of product_id
### Total revies per category
- Rows: Category
- Values: Sum of rating_count
## DASHBOARD LAYOUT
- Charts:
   - Bar: Average Discount by Category
   - Column: Average Actual vs Discounted Price

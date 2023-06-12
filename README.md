# Home_Sales

The goal of this project is to use SparkSQL to analyze home sales data and calculate key metrics. The project involves the following steps:

1. Import the necessary PySpark SQL functions and read the home_sales_revised.csv data into a Spark DataFrame.

2. Create a temporary table called "home_sales" to enable querying using SparkSQL.

3. Use SparkSQL to answer the following questions:
   - Calculate the average price for a four-bedroom house sold for each year.
   - Calculate the average price of a home for each year it was built that has three bedrooms and three bathrooms.
   - Calculate the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet.
   - Determine the "view" rating for homes costing more than or equal to $350,000 and measure the query's runtime.

4. Cache the temporary table "home_sales" to improve query performance.

5. Check if the temporary table is cached.

6. Run a query on the cached data to filter out view ratings with an average price greater than or equal to $350,000. Measure the query runtime and compare it to the uncached runtime.

7. Partition the home sales data by the "date_built" field and save it in Parquet format.

8. Create a temporary table for the Parquet data.

9. Run the query from step 6 on the Parquet temporary table. Measure the query runtime and compare it to the uncached runtime.

10. Uncache the "home_sales" temporary table.

11. Verify that the "home_sales" temporary table is uncached using PySpark.

The project requires creating a Spark DataFrame, creating temporary tables, writing SparkSQL queries to calculate metrics, caching and uncaching tables, and analyzing query runtimes. The final step is to download the completed notebook and upload it to the "Home_Sales" GitHub repository.

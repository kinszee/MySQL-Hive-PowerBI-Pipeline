# MySQL-Hive-PowerBI-Pipeline

The project aims to create 3 dashboards for a client's Pizza restuarant. The client has requirements to show 
1. Order Activity
2. Inventory Management
3. Staff management

Summary: To build an end to end pipeline, I Created tables in MySQL DB, ingested tables to Hadoop for data warehousing and built HiveQL views. Hive views in Linux VM were connected to Power BI application in Windows to 
create visualizations.

*PROJECT GOALS*
- Create normalized database schema in MySQL
- Build analytical Hive database on top of MySQL data
- Develop HiveQL views for reporting
- Connect Hive to Power BI using ODBC driver
- Create interactive Power BI dashboards and reports

*REQUIREMENTS*
> Data Model Requirements
* MySQL DB with address, customers, ingredient, inventory, item, orders, recipe, rota, shift and staff tables
* Hive DB with external tables matching MySQL schemas
* Hive views to join data for analysis
* Referential integrity between MySQL tables
  
> Dashboard Requirements
* Ability to filter by date, time, item and staff name.
* Interactive reports in Power BI for:
  * Order Activity
     * i) Total Orders
     * ii) Total Sales
     * iii) Total items
     * iv) Average Order Value
     * v) Sales by category
     * vi) Top 5 selling Items
     * vii) Orders by hour
     * viii) Sales by hour
     * ix) Orders by Address
     * x) Orders by delivery/pick up
       
  * Inventory Management
    * i) Total quantity by Ingredient
    * ii) Total Cost of Ingredients
    * iii) Calculated Cost of Pizza
    * iv) Percentage stock remaining by ingredient
    * v) List of ingredients to re-order based on remaining inventory

  * Staff Management
    * i)  Total Staff Cost
    * ii) Total hours worked
    * iii) Hours worked by individual staff members
    * iv) Cost per staff member
       

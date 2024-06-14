Fact Tables:
Forecast:

-Date: The date for which the forecast is made.
-IT Department: The IT department responsible for the forecasted cost.
-Cost Element: The element for which the cost is forecasted.
-Country: The country associated with the forecast.
-Forecast: The forecasted cost value.

Budget:

-Date: The date for which the budget is set.
-IT Department: The IT department responsible for the budgeted cost.
-Cost Element: The element for which the budget is set.
-Country: The country associated with the budget.
-Budget: The budgeted cost value.

Actuals:

-Source Name: The name of the source of the actual cost.
-Date: The date on which the actual cost was recorded.
-IT Department: The IT department responsible for the actual cost.
-Cost Element: The element for which the actual cost was recorded.
-Country: The country associated with the actual cost.
-Actual: The actual cost value.

Lookup Tables:

CostElements:

-Cost Element: The primary key.
-Cost Element Area: The area associated with the cost element.
-Cost Element Group: The group to which the cost element belongs.
-Business Area: The business area associated with the cost element.

Departments:

-IT Department: The primary key.
-IT Area: The area associated with the IT department.
-Dept. Manager: The manager of the department.

Regions:

-Country: The primary key.
-Region: The region associated with the country.
-Dimension Tables:
-To effectively create dimension tables, you need to flatten the lookup tables into dimensions that can be used in your star schema.

Dim_CostElement:

-Cost Element: Primary key.
-Cost Element Area
-Cost Element Group
-Business Area

Dim_Department:

-IT Department: Primary key.
-IT Area
-Dept. Manager

Dim_Region:

-Country: Primary key.
-Region


# 1. Load and Connect the table in format of text/csv:

 1.1: Also connect the folder in power BI then combine the tablesa nd load them as one. everything wiil be ordered in cronological order for us 



#  2. Cleaning the data:

 2.1 Enables View -> Column Quality to see the valid, error and empty values for each column.


Before visualization:

Create relationship
Create date master table

Delete column named Source.Name from Actuals table.

Change the category of Country column from Forecast Table: for easily mapping
	Column Tool -> Data Category -> Choose country

Change the category of Country column from Budget Table: for easily mapping
	Column Tool -> Data Category -> Choose country


Delete unnecessary columns from Dim Tables


 

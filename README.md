# HR-analysis-using-PowerBI
## Step 1: Load the Data into Power BI
Import Tables: Start by loading the required datasets (e.g., Performance Rating, Satisfaction Level, Employee, Education, and States tables) into Power BI. You can do this by selecting the “Get Data” option and choosing the appropriate data source (e.g., Excel, CSV, SQL Server).
Preview and Clean Data: Once the tables are loaded, preview the data in Power Query Editor. Make any necessary adjustments (e.g., remove nulls, duplicates, or fix data types).
## Step 2: Open the Data Model View
Navigate to the Model View: After loading the tables, switch to the Data Model view (by selecting the “Model” icon from the left panel) where all the imported tables are visible.
## Step 3: Establish Relationships Between Tables
Identify Common Fields: Look for common columns between the tables to establish relationships. For example:
Performance Rating Table: Can be connected to the Satisfaction Level and Performance Level tables through a common field, like an Employee ID or Rating ID.
Employee Table: Can be linked to the Education and States tables using fields such as Employee ID or State Code.
Drag and Drop to Connect: Click and drag the common column from one table to the related table to create the relationship.
Example: Drag the Employee_ID from the Performance Rating table to the Employee_ID in the Employee table.
## Step 4: Set Relationship Types (Mostly Many-to-One)
Check and Adjust Relationship Types: Power BI automatically sets the relationship type when you connect two tables. However, ensure that it reflects a "many-to-one" relationship where needed.
Example: The Employee table (one) can have multiple records in the Performance Rating table (many). Therefore, a many-to-one relationship is ideal here.
To adjust, click on the relationship line, and in the "Manage Relationships" pane, you can edit the relationship type and cardinality.

![Screenshot (275)](https://github.com/user-attachments/assets/0e0c1678-a6b5-402c-ad0f-fc4b4cced327)

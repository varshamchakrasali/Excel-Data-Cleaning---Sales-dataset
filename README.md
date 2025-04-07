# Excel-Data-Cleaning---Sales-dataset

✅ 1. Handle Missing Values
Objective: Identify and handle empty or null cells in the dataset.

Steps:

- Apply filters to all columns (Data → Filter).

- In each column’s dropdown, check if "(Blanks)" appears.

- If blanks are present:

 - Manually fill them with appropriate values (if known), OR Delete the columns which are not helpful in analysing and which has more null values 

- Delete rows with missing critical data using Go To Special → Blanks → Delete Rows


✅ 2. Remove Duplicate Rows
Objective: Eliminate duplicate records to ensure data integrity.

Steps:

Select all data (Ctrl + A).

Go to Data → Remove Duplicates.

Check all columns to compare entire rows.

Click OK to remove duplicates.


✅ 3. Standardize Text Values

Objective: Clean inconsistent capitalization and spacing in text columns like STATUS, PRODUCTLINE, and COUNTRY.
Steps: 
- Standardizing status column - TRIM() removes leading/trailing spaces.
LOWER() converts text to lowercase (e.g., "Shipped" → "shipped").

- Standardizing the COUNTRY column - TRIM() removes leading/trailing spaces.
- UPPER() ensures all values are capitalized (e.g., "usa" → "USA").
- CONCATENATE() Merging of 2 functions 

✅ 4. Convert Date Formats

Objective: Make all date entries follow a consistent format (dd-mm-yyyy).
Steps:
-Select the ORDERDATE column.
-Press Ctrl + 1 → Format Cells → Custom.
-Set the Custom format as: dd-mm-yyyy

✅ 5. Rename Column Headers

Objective: Ensure column names are clean, lowercase, and without spaces.
Steps:
-Manually rename the headers in Row 1.
-Example: Order Date → order_date
-Remove special characters or extra whitespace.

✅ 6. Check and Fix Data Types

Objective: Ensure numerical, date, and text columns are using the correct data types.
Steps:
Use =ISNUMBER(), =ISTEXT(), or =ISDATE() 


🔍 Excel Functions Used
Function	Purpose
TRIM()	Removes extra spaces
LOWER()	Converts text to lowercase
UPPER()	Converts text to uppercase
PROPER()	Capitalizes first letter of each word
VALUE()	Converts text to numeric values
ISNUMBER()	Checks if a value is a number
ISTEXT()	Checks if a value is text
ISDATE()	(via formatting) Checks for valid dates

# Global-Sales-Dashboard
Interactive Excel dashboards to visualize revenue and profit data for a global sales company

## Project Overview
This project focuses on creating interactive Revenue and Profit Dashboards for a Global Sales Company using Microsoft Excel. The goal is to enhance data accuracy, interactivity, and meaningful insights by applying various data cleaning, transformation, and visualization techniques to enhance the user experience. Both raw and processed data are stored in separate sheets for easy reference. 

## How to Use

1. Clone the repository and download the Excel file.

2. Open the file in Microsoft Excel.

3. Explore the cleaned dataset and dashboards.

4. Interact with slicers to filter data dynamically.

## Steps to build the Dashboards

### 1. Data Injection 

The data was loaded into Excel from a CSV file. ensuring the correct delimiter was detected and columns were appropriately aligned 

### 2. Understanding the Data 

Familiarized with the data structure by reviewing the rows and columns, key variables and their data types and identified the purpose. 

### 3. Data Inspection 

i) Missing values identified in both numerical and categorical columns 

ii) Duplicate entries detected in the dataset. 

iii) Presence of outliers affecting data consistency are identified 

iv) Calculation errors observed in derived or computed fields. 

v) Unstandardized text formats, including inconsistent capitalization. 

vi) Incorrect formatting for date and currency fields are noted. 

### 4. Data Cleaning 

#### i) Removing Duplicates: 

  a. Duplicate rows were identified and removed using the Remove Duplicates option in Excel. 
  
  b. Relevant columns were selected to check for duplicates, and a summary confirmed the number of duplicates removed. 

#### ii) Handling Missing Values: 

  a. Blank cells were identified by FILTER 
  
  b. Numerical Columns: Blank cells are replaced with the Mean of the respective columns. 
  
  c. Categorical Columns: The most frequent value (Mode) was used to replace missing entries. 
  
  d. Regions: Missing "Region" values were filled using VLOOKUP by referencing the "Country" column. 

#### iii) Standardizing Text Capitalization: 

  a. Inconsistent text formats in columns like "Region", "Country", "Sales Channel", "Order Priority" were identified. 
  
  b. Function PROPER was applied to ensure uniform capitalization. 
  
  c. "USA" was converted to full capitalization using Find and Replace. 

#### iv) Fixing Calculation Errors: 

  Errors in calculated fields like total revenue, cost, and profit were identified and corrected using accurate formulas. 

#### v) Handling Outliers: 

  a. Outliers were identified using the Z-score method, where values with a Z-score above 3 or below -3 were considered extreme. 
  
  b. The identified outliers were replaced with the mean value of the dataset to maintain consistency. 

#### vi) Correcting Formats: 

  Incorrect date and currency formats were standardized for consistency across the dataset. 

#### vii) Verifying Data Consistency: 

  a. Final review of the dataset was conducted to ensure all corrections were applied correctly. 
  
  b. The cleaned and validated dataset was saved as a new file for future use. 

### 5. Data Transformation 

#### i) Conditional Formatting: 

  a. Different colors scales were used to distinguish between Critical, High, Medium, and Low priority levels from Order Priority column, making it easier to visually identify the urgency of each order. 
  
  b. In Total Profit column, profits greater than or equal to 5000 were highlighted with green font, and losses (negative values) were highlighted with red font. This makes it easy to quickly spot profitable and loss-making orders 

#### ii) Data Extraction: 

  The Order Year and Order Month were extracted from the Order Date by Split Text to Columns feature and then converted month from numbers into words by formula.  

Note: The raw data and processed data are added as separate sheets to the excel file 

### 6. Exploratory Analysis - Reports Creation  

Built reports to summarize and analyze key metrics like total revenue, profit, sales by region, and product categories by using: 

i) Pivot Tables: Grouped and filtered data effectively for focused insights. Used calculated fields to derive new metrics directly within pivot tables.  

ii) Pivot Charts: Visualized trends and patterns by creating charts such as bar graphs, line charts, pie charts etc. 

### 7. Data Visualization – Interactive Dashboards 

i) Merged multiple charts to create 2 different cohesive dashboards for Revenue and Profit. 

ii) Made it interactive by adding slicers to filter data dynamically based on user input, such as regions, order priorities, or product categories etc. 





 

 

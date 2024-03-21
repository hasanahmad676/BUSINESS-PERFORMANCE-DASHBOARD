
# BUSINESS PERFORMANCE DASHBOARD

### Dashboard Link : https://app.powerbi.com/groups/me/reports/2e332c44-892e-4f81-8519-323192512b54/ReportSection

## Problem Statement

This dashboard helps the company to understand their product, their sales, profit, gross sales, COGSand their otherthing better. It helps the company to know their sales in the year of 2013 and 2014 according to each month. they could also know their year over year (YoY) sales ,profit, gross sales and cogs. They can see top 3 product by segment profit with their product name sales, gross sales and sales. They can also know the sales of 2013 and 2014 according to the country.
By using this they can increase their productivity.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a Excel file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present in the dataset.
- Step 5 : For calculating Total sales,Total profit,gross sales,cogs, sales by country within 2013 and 2014.
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Since we want to see the sales according to year of 2013 and 2014 i have to extract the  date column and take only the year of 2013 and 2014 sales value and create new column using Dax. 
for creating new column following DAX expression was written;
    
    Total Sales 2013 = 
       CALCULATE(
            SUM(financials[ Sales]),
            YEAR(Financials[Date]) = 2013

    Total Sales 2014 = 
        CALCULATE(
            SUM(financials[ Sales]),
            YEAR(Financials[Date]) = 2014
)
)
        
          
Snap of new calculated column ,

![s3](https://github.com/hasanahmad676/BUSINESS-PERFORMANCE-DASHBOARD/assets/82166280/6ae67290-fb31-4eed-93d0-141dd2bf19f0)

- Step 8 : Visual filters (Slicers) were added for four field named "country","Discount Brand","product" and "segment".

![s4](https://github.com/hasanahmad676/BUSINESS-PERFORMANCE-DASHBOARD/assets/82166280/eb8af2c9-7948-4b22-960c-75b11b9c2630)

- Step 9 : Four card visuals were added to the canvas, they represent the gross sales,total sales,total profit  and cogs.

![s5](https://github.com/hasanahmad676/BUSINESS-PERFORMANCE-DASHBOARD/assets/82166280/5c9c7154-0fd6-458d-af73-5cbd58f73dc7)

- step 10 : we used a table where we findout the top 3 product by segment using unsold unit of product.


![s6](https://github.com/hasanahmad676/BUSINESS-PERFORMANCE-DASHBOARD/assets/82166280/d3dc9cf6-3a8f-4848-ba19-bd625f977933)

- step 11 : we also use a cluster bar chart where we calculate the total sales according to the month for the year of 2013 and 2014.

![s7](https://github.com/hasanahmad676/BUSINESS-PERFORMANCE-DASHBOARD/assets/82166280/2a44be69-c3e3-4462-a31d-1f8381ee3daf)


- Step 11 : In the report view, under the insert tab, using shapes option from elements group a rectangle was inserted where title added to the report design area. 


- Step 18 : The report was then published to Power BI Service.
 

![s1](https://github.com/hasanahmad676/BUSINESS-PERFORMANCE-DASHBOARD/assets/82166280/024f08e9-7a2e-41d4-80a8-4d66060165ff)

# Snapshot of Dashboard (Power BI Service)


![s8](https://github.com/hasanahmad676/BUSINESS-PERFORMANCE-DASHBOARD/assets/82166280/61c36479-3ad4-4598-9748-5cb4a94af47b)

# Report Snapshot (Power BI DESKTOP)


![s2](https://github.com/hasanahmad676/BUSINESS-PERFORMANCE-DASHBOARD/assets/82166280/48ce8605-7de4-4f0b-929b-5802ad4a7b63)

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;


### [1] Total Gross Sales
     
      Here we findout that total gross sales is 128 million.
 

### [2] Total Sales
 
       Here we findout that total sales is 119 million.


### [3] Total Profit 
       Here we findout that total sales is 17 million.

### [4] Total COGS 
        
        Here we findout that total COGS  is 102 million.

### [4] YEAR over YEAR gross sales, sales, profit and COGS.
        1. YEAR over YEAR gross sales is 348%
        2. YEAR over YEAR  sales is 349%
        3. YEAR over YEAR Profit is 336%
        4. YEAR over YEAR gross COGS IS 352%

### [6] TOP 3 PRODUCT BY segment USINGH UNSOLD unit.
       
       1. Small Business
       2. Channel Partners
       3. Midmarket

### [7] Total sales of 2014 and 2013 by month.  
### [8] Total sales of 2014 and 2013 by country.     
 

        

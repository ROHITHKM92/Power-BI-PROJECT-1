# Global Super Store: 2016 Sales Analysis Overview 🌐💼



## Introduction 🚀

Upon discovering this online dataset, I was captivated by its richness, providing an excellent opportunity for honing my data cleaning, analysis, and visualization skills.

**Applied Power BI Concepts:**
- **DAX Concepts:** Calculated column, Custom Column, Year(), IF().
- **Data Modeling:** Star Schema (*:1)

----

## Problem Statement 🤔

- How swiftly are orders delivered on average?
- Unveiling the yearly sales saga since 2012: Is there a steady ascent?
- Who are the powerhouse customers?
- Profits and losses: Product-wise revelations.
- Delving into more data-driven insights from our sales numbers.

## Data Sourcing 📊

Armed with questions, I acquired the dataset by downloading the CSV file, unleashing it into Power BI for a meticulous journey of cleaning, analysis, and visualization.

It comprises three tables:
1. **ORDERS:** 51,291 rows, 24 columns
2. **PEOPLE:** 24 rows, 2 columns
3. **RETURNS:** 1,079 rows, 3 columns

----

## Data Transformation/Cleaning 🧹

Utilizing the Power Query Editor in Power BI, the data underwent a transformative journey. [See screenshot for applied steps]

Key steps included:
- Setting the first row as headers in the PEOPLE and RETURNS tables.
- Analytical transformation of the 'ORDER' table:
  - Calculation of 'delivery days' using "custom columns": `delivery days = [shipped date] - [order date]`
  - Creation of a new column for the year of the order date: [Order Year]
  - Addition of a conditional column to the 'RETURNS' table to assign a numeric value to the 'Returned' response (YES: 1, NO: 0).
  - Changing datatype from 'TEXT' to 'WHOLE NUMBER'.

## Data Modeling 🎨

Power BI wove connections between tables, crafting a star schema model. The 'Order' table takes center stage as the fact table, with 'Return' and 'People' tables gracefully linked via common columns: 'order ID' and Region, respectively. 
![model_view](https://github.com/ROHITHKM92/Power-BI-PROJECT-1/assets/87298902/636c4413-4df9-4a79-8e57-c9d6c61c3a43)

## Data Analysis and Visuals 📈


![DB1](https://github.com/ROHITHKM92/Power-BI-PROJECT-1/assets/87298902/62d23f0c-6030-4f2e-b96d-e719c2f8da19)
Noteworthy Insights:
1. The average delivery time per product on every order is a swift 4 days.
2. The sales narrative unfolds: 2012 = $2.26M, 2013 = $2.68M, 2014 = $3.41M, 2015 = $4.30M.
3. The crown for the highest sales sits atop the Western Europe region, commanding almost $450K.

![g1](https://github.com/ROHITHKM92/Power-BI-PROJECT-1/assets/87298902/b6c70127-6afc-4902-8f59-f373f838da7e)

- Raymond Buch is the most valuable customer by 2015 sales.

## Conclusions & Recommendations 📝

- Orders dance to the tune of a 4-day delivery.
- The sales crescendo has been a gradual ascent since 2012, at a mesmerizing rate of approximately 19%.
- Different customers wear the profit crown each year.
- Tamara Chand shines as the beacon of sales brilliance from 2012 to 2015. Yet, in 2012, Sanjit Chand claimed the sales throne.
- The sales symphony continued with standout performances by Mike Gokenbach (2013), Tamara Chand (2014), and Raymond Buch (2015).
- The product 'Canon Image (Class 2200) advance copier' harmonized the highest profits in 2014 and 2015.
  
Additional Harmonies:
- Over 50% of total sales come from the consumer segment.
- The Asia Pacific region boasts the highest sales crescendo.

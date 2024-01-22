
# Project Name: YouGov New Year's Resolutions Analysis







## Overview: 

This project aims to analyze New Year's resolutions data obtained from YouGov's public PDF. The analysis involves data preparation using Power BI, followed by visualization to explore insights related to resolutions and demographics.

## Data Preparation: 
### 1. Importing Data
• Utilize the PDF connector in Power BI to extract data from the YouGov PDF.

• Select relevant tables: Table008, Table009, Table010, and Table011.

### 2. Unpivoting Data
• Unpivot the selected tables to consolidate demographic attributes into a single column.

### 3. Combining Tables (Making Resolutions)
• Combine Table008 and Table009.

• Create columns: [Making Resolutions], [Attribute], [Percent].

• Remove "Totals" and "UnweightedN" from the Making Resolutions column.

• Replace values in the Making Resolutions and Attribute columns for user-friendly labels.

### 4. Combining Tables (Top 5 Resolutions)

• Combine Table010 and Table011.

• Create columns: [Resolution], [Attribute], [Percent].

• Remove "Totals" and "UnweightedN" from the Resolution column.

• Replace values in the Resolution and Attribute columns for user-friendly labels.

### 5. Creating Attribute Categories

• Generate a new table with distinct values from the Attribute column.

• Add a column grouping Attributes into categories (e.g., gender, household income, age).

    
## Data Visualization:
### 1. Likelihood of Making Resolutions (100% Stacked Bar Chart)

• Attribute on the y-axis, percent from "Making Resolutions" on the x-axis, and Making Resolutions in the legend.

• Title: "Likelihood of Making Resolutions."

• Set transparency to 25% for bar color fill.

• Enable borders on bars matching the bar color.

### 2. Top 5 Resolutions (Bar Chart)

• Resolution on the y-axis, percent from Resolutions on the x-axis.
Title: "Top 5 Resolutions."

• Apply transparency to 25% for bar color fill.

• Enable borders on bars matching the bar color.

### 3. Filtering Top 5 Resolutions Chart

• Filter the chart to show only the top 5 resolutions based on the selected attribute in the Likelihood of Making Resolutions chart.

• Display more than 5 values in the case of ties.

### 4. Slicer for Demographic Category

• Add a slicer allowing single-select of a demographic category for attribute display in the Likelihood of Making Resolutions chart.

### 5. Data Labels on Top 5 Resolutions Chart

• Show percent value for each resolution.

• Add a detail data label:

    • If attribute selected, compare percent values to the total group.
    • If no attribute selected, compare percent values to the first Attribute value.
## Dataset:
This project uses data sourced from the YouGov New Year's Resolutions poll results PDF, accessible at YouGov New Year's Resolutions Poll Results. It can be accessed at https://d3nkl3psvxxpe9.cloudfront.net/documents/New_Year_s_Resolutions_poll_results.pdf
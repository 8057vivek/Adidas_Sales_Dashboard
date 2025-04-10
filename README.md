---
title: "Adidas US Sales Power BI Dashboard"
---

![](dashBoardImage)

# 📊 Adidas US Sales Power BI Dashboard

## 📁 Dataset: `Adidas_US_Sales_Processed.xlsx`

This dataset contains sales information for **Adidas products sold across the United States**, capturing data from different regions, states, cities, and sales methods.

### 🔍 Dataset Columns

| Column Name        | Description                                         |
|--------------------|-----------------------------------------------------|
| `sales_id`         | Unique identifier for each sale                     |
| `retailer`         | Name of the retail company                          |
| `retailer_id`      | ID of the retailer                                  |
| `invoice_date`     | Date of the sale                                    |
| `region`           | US region (e.g., Northeast, South)                  |
| `state`            | US state where the sale occurred                    |
| `city`             | City of the sale                                    |
| `product`          | Type of Adidas product                              |
| `price_per_unit`   | Selling price per unit                              |
| `units_sold`       | Number of units sold                                |
| `total_sales`      | Revenue from the sale                               |
| `operating_profit` | Profit from the sale                                |
| `sales_method`     | Channel through which sale occurred (e.g., Online)  |

---

## 📈 Power BI Dashboard Overview

This interactive dashboard visualizes Adidas' performance across various dimensions using slicers, charts, and KPIs.

### 🔹 Top Summary Cards (KPIs)

- **Total Sales**: $120M  
- **Total Profit**: $33M  
- **Total Units Sold**: 2M  

### 🔹 Slicers for Interactivity

- **Sales/Profit Toggle Buttons**  
  Allows dynamic switching between sales and profit measures for visualizations.
  
- **Gender Button Slicer (Men/Women)**  
  Filters the category selection panel based on selected gender.

- **Product Category Filter**  
  Dependent slicer based on gender, shows:
  - Men's Apparel
  - Men's Athletic Footwear
  - Men's Street Footwear

- **Sales Method Filter**  
  Choose from:
  - In-store
  - Online
  - Outlet

---

## 📊 Visualizations Used

1. **Retailer-Wise Performance Table**  
   Tabular data with sparklines and profit margins.

2. **Bar Chart** - *Total Sales by Product Category*  
   Highlights top-selling categories.

3. **Line Chart** - *Total Sales by Quarter (2020-2021)*  
   Compares quarterly sales trends.

4. **Donut Chart** - *Sales by Sales Method*  
   Visual distribution of sales by channel.

5. **Treemap** - *Sales by Region*  
   Shows contribution of each region to total sales.

6. **Map Visual** - *Total Sales by State*  
   Location-based view of total sales with color-coded bubbles.

7. **Line Chart** - *Year-over-Year Growth by Month*  
   Monthly growth in total sales from Jan 2021 to Dec 2021.

---

## 🧠 DAX Measures & Logic

- **Dynamic Measure Switching**:  
  Used `SELECTEDVALUE` and `SWITCH` DAX to toggle between Total Sales and Profit based on button click.

- **Dynamic Titles**:  
  Used selected slicer values in DAX to dynamically generate titles like:  
  `Total Sales by Region` or `Total Profit by Category`.

- **Gauge Chart Logic**:  
  Custom total values (e.g., for 100%) set using DAX for max thresholds in gauge charts.

---

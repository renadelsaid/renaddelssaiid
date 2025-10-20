# renaddelssaiid
# FNP Sales Data Analysis

## Overview

This repository contains the **FNP Sales Dataset (`fnpsales.xlsx`)**, a structured dataset designed for business intelligence, data analytics, and visualization projects. The dataset captures detailed information about customer orders, product performance, and revenue across multiple locations and occasions. It is particularly suitable for building **Power BI dashboards**, **ETL pipelines**, or conducting **sales performance analysis**.

---

## File Description

### 📘 `fnpsales.xlsx`

The Excel file contains multiple sheets, representing both **fact** and **dimension** tables commonly used in analytical data models.

| Sheet Name | Description |
|-------------|--------------|
| **orders** | Fact table containing transactional order-level data, including order details, revenue, and delivery times. |
| **customer** | Dimension table with customer demographics and contact details. |
| **product** | Dimension table containing product information, pricing, and category classification. |
| **Sheet3** | Aggregated summary table or pivot output for exploratory analysis and reporting. |
| **Sheet5** | Raw export of order and revenue data (first 1000 rows). |
| **dashboard** | Placeholder sheet for Power BI or Excel dashboard visualizations. |

---

## Data Schema

### **orders**
| Column Name | Description |
|--------------|-------------|
| `Order_ID` | Unique identifier for each order. |
| `Customer_ID` | Foreign key linking to the Customer dimension. |
| `Product_ID` | Foreign key linking to the Product dimension. |
| `Quantity` | Number of items ordered. |
| `Order_Date` | Date when the order was placed. |
| `Delivery_Date` | Date when the order was delivered. |
| `Revenue` | Total order revenue (in INR). |
| `Price (INR)` | Price per unit of product. |
| `Occasion` | Occasion or event associated with the order (e.g., Diwali, Anniversary). |
| `Location` | Delivery location. |
| `Month Name` | Month extracted from the order date for reporting. |
| `diff/ delivery& order` | Time difference (in days) between order and delivery. |
| `Day Name(order)` | Day of the week when the order was placed. |

### **customer**
| Column Name | Description |
|--------------|-------------|
| `Customer_ID` | Unique customer identifier. |
| `Name` | Full name of the customer. |
| `City` | Customer’s city. |
| `Contact_Number` | Customer contact number. |
| `Email` | Customer email address. |
| `Gender` | Gender of the customer. |
| `Address` | Complete mailing address. |

### **product**
| Column Name | Description |
|--------------|-------------|
| `Product_ID` | Unique product identifier. |
| `Product_Name` | Name of the product. |
| `Category` | Product category (e.g., Plants, Sweets, Soft Toys). |
| `Price (INR)` | Unit price in Indian Rupees. |
| `Occasion` | Primary occasion for which the product is suitable. |
| `Description` | Brief text description of the product. |

---

## Use Cases

- **Power BI Dashboard Development:** Create interactive reports tracking sales by month, occasion, and region.
- **ETL & Data Warehousing:** Use as a base for star schema modeling.
- **Data Analytics Projects:** Analyze revenue trends, delivery performance, and customer behavior.
- **Machine Learning Applications:** Predict order volumes or customer lifetime value.

---

## Suggested Tools

- **Power BI / Tableau** – for visual dashboards  
- **Python (pandas, matplotlib)** – for data preprocessing and analysis  
- **SQL / DAX** – for data modeling and metric calculations  

---

## License

This dataset is intended for **educational and analytical purposes**. Redistribution or commercial use should credit the original author or data source if applicable.


---

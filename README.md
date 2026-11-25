# Usman’s Dash & Dine — Restaurant Sales & Delivery Analytics

## Project Overview

**Usman’s Dash & Dine** is an end-to-end Power BI data analytics project focused on analyzing the sales performance, customer behavior, menu performance, and delivery operations of a  delivery-only fast-food restaurant based in Peshawar, Pakistan.

The project uses a  dataset covering the period **January 1, 2025, to December 31, 2025**. It demonstrates how raw business data can be transformed into meaningful insights through data validation, data modeling, DAX calculations, and interactive dashboard development.

**Currency:** Pakistani Rupee (PKR)  
**Business Location:** Peshawar, Pakistan  
**Analysis Period:** 2025  


## Business Objectives

The main objectives of this project are to:

- Analyze restaurant sales and revenue performance.
- Identify the best-performing menu categories and products.
- Understand customer ordering activity.
- Evaluate payment method preferences.
- Compare order volumes across delivery zones.
- Analyze delivery times and operational performance.
- Monitor completed, cancelled, and refunded orders.
- Build an interactive dashboard to support business decision-making.

## Dataset Description

The project contains four CSV files with the following structure:

| Dataset | Records | Columns |
|---|---:|---:|
| Customers | 800 | 6 |
| Menu_Items | 60 | 7 |
| Orders | 2,500 | 9 |
| Order_Details | 4,500 | 7 |
| **Total** | **7,860** | **29** |

### Dataset Details

**1. Customers.csv**

Contains customer information, including customer ID, name, city, customer type, registration date, and gender.

**2. Menu_Items.csv**

Contains menu information, including item ID, item name, category, size, unit cost, selling price, and availability.

**3. Orders.csv**

Contains order-level information, including order ID, customer ID, order date, order time, delivery zone, payment method, order status, delivery fee, and delivery time.

**4. Order_Details.csv**

Contains individual order-item records, including order detail ID, order ID, item ID, quantity, unit price, discount amount, and line total.

## Data Model

The project uses a relational data model with four main tables and a dedicated Date table.

### Relationships

- Customers → Orders (One-to-Many)
- Orders → Order_Details (One-to-Many)
- Menu_Items → Order_Details (One-to-Many)
- Date → Orders (One-to-Many)

The model supports analysis across customers, orders, menu items, and time.

## Data Cleaning & Validation

Data preparation and validation were performed using Power BI Power Query Editor.

Key validation activities included:

- Checking primary key uniqueness.
- Validating foreign key relationships.
- Checking missing values and data errors.
- Validating order quantities and financial values.
- Verifying line totals against quantity, unit price, and discounts.
- Checking customer classifications against order history.
- Investigating historical orders containing currently unavailable menu items.
- Validating date and time columns.
- Checking delivery fees and delivery time values.

All four original datasets were retained during validation.

## Key Performance Indicators (KPIs)

The dashboard includes 12 KPI cards:

1. Total Orders
2. Total Revenue
3. Completed Orders
4. Cancelled Orders
5. Refund Orders
6. Average Order Value (AOV)
7. Total Items Sold
8. Cancellation Rate
9. Unique Customers
10. Total Customers
11. Average Delivery Time
12. Total Discount Given

Revenue, completed orders, items sold, average order value, and average delivery time are calculated using completed orders where applicable.

## Dashboard Pages

The Power BI report is organized into three pages.

### Page 1 — Executive Overview

Provides a high-level view of overall restaurant performance.

**Includes:**
- 12 KPI cards
- Monthly Revenue Trend
- Date Range slicer

### Page 2 — Sales & Menu Analysis

Focuses on revenue performance, menu categories, products, and payment preferences.

**Visualizations:**
- Revenue by Menu Category
- Revenue by Payment Method
- Items Sold by Category and Size
- Top 10 Best-Selling Menu Items
- Menu Category slicer

### Page 3 — Delivery & Operations

Focuses on delivery performance and operational efficiency.

**Visualizations:**
- Orders by Delivery Zone
- Average Delivery Time by Zone
- Orders by Hour of Day
- Order Status Breakdown
- Average Delivery Time vs Target (Gauge)
- Delivery Zone slicer

The report uses interactive slicers to allow users to explore different aspects of restaurant performance.

## Tools & Technologies

- **Microsoft Power BI Desktop** — Data modeling, DAX, visualizations, and dashboard development.
- **Power Query Editor** — Data cleaning and validation.
- **DAX** — KPI calculations and analytical measures.
- **CSV** — Source data format.
- **GitHub** — Project documentation and portfolio presentation.

## Business Value

This project demonstrates how restaurant data can be used to:

- Identify high-performing menu categories and products.
- Understand revenue and customer ordering patterns.
- Monitor cancellations and refunds.
- Compare delivery-zone performance.
- Identify periods of higher order activity.
- Monitor delivery efficiency against a proposed operational target.

The dashboard provides a consolidated view of restaurant performance and demonstrates practical business intelligence and data analytics skills.

## Important Note

This project uses **synthetic data created for analytical and portfolio purposes**. It does not represent the actual operations or financial performance of a real restaurant.

The 38-minute delivery target used in the gauge is a proposed business benchmark, not a measured historical target.

## Project Status

Dashboard development and analytical implementation are the focus of this project.


## Name:Sumedha Gopinath Karpe
# College name : AVCOE

## PROJECT TITLE:Farm Produce Inventory and Sales Tracking System
## Overview
This system is designed to manage farm produce inventory, track sales, and manage restocking. The goal is to help farmers, suppliers, and store managers efficiently handle produce stocks, record sales, generate sales reports, and be alerted when stocks run low.

## Features
Inventory Management: Track the quantity and prices of farm produce.
Sales Management: Record sales transactions and update inventory automatically.
Sales Reporting: Generate reports on total sales and revenue per produce.
Restock Alerts: Receive automatic alerts when the inventory for a particular produce falls below a set threshold.
Supplier Management: Link farm produce with their suppliers for easy tracking.
System Components
## Tables:

# Produce: Stores information about different types of produce (e.g., name, category).
### 1.Suppliers: Contains information about suppliers for each produce.
### 2.Inventory: Manages the stock quantity and unit price of each produce.
### 3.Sales: Records each sale transaction, including the quantity sold and total price.
### 4.Customers: Holds data on customers who purchase the produce.
## Stored Procedures:

### 1.Add_Sale: Records a sale transaction and updates inventory.
### 2.Generate_Sales_Report: Generates a summary of total sales and revenue per produce.
### 3.Restock_Inventory: Restocks inventory for a given produce by adding new stock or updating existing stock.
## Triggers:

### 1.Update_Inventory_After_Sale: Automatically updates the inventory after a sale is made.
### 2.Low_Stock_Alert: Sends an alert if stock for a particular produce goes below a certain threshold.
## Installation and Setup
Create Database Tables: Set up the database by creating tables for Produce, Suppliers, Inventory, Sales, and Customers.
Define Stored Procedures: Implement stored procedures to handle sales, report generation, and inventory restocking.
Implement Triggers: Set up triggers to automatically update inventory and send alerts when stock levels are low.
Usage
1. Add a Sale:
This procedure records a sale and updates the inventory. A sale will decrease the stock of the produce and log the transaction.

2. Generate a Sales Report:
Run a report to see the total quantity of each produce sold, along with the total revenue generated.

3. Restock Inventory:
Restock the inventory when supplies are running low. This procedure updates the inventory for a specific produce or inserts new stock records.

4. Low Stock Alerts:
Whenever a sale causes stock levels to fall below a predefined threshold, an alert is generated.

Testing
Sales Transactions: Test the system by adding sales and ensuring the inventory is updated.
Stock Updates: Restock inventory and verify that the system correctly updates stock.
Report Generation: Run the sales report and verify it correctly aggregates sales data.
Trigger Functionality: Check that the low stock alert triggers correctly when inventory falls below the set threshold.
Conclusion
This system efficiently handles the tracking of farm produce, sales, and inventory. By automating inventory updates and generating real-time sales reports, it ensures seamless management and helps users keep track of stock levels and revenue.


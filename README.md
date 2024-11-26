# Amazon Trade: Shipping Analytics Dashboard

## Project Description

Amazon Trade is a global FMCG (Fast Moving Consumer Goods) shipping company. This project aims to provide the **Shipping Manager** with a comprehensive dashboard to track monthly order processing and shipping. The dashboard offers visibility into:
- The number of orders processed and shipped daily.
- Outstanding orders that need to be shipped.
- Geographic distribution of shipping activities.

---

## Objectives
1. **Order Tracking:**
   - Provide a daily count of orders processed, shipped, and outstanding for a selected month.
2. **Shipping Insights:**
   - Visualize the geographic locations where orders are shipped and identify regions with outstanding orders.
3. **Data Accessibility:**
   - Connect to data hosted on MariaDB and Azure or utilize provided CSV files for analysis.

---

## Key Insights from April 2020 Analysis

### **1. Order Processing Overview**
- **Total Orders (April 2020):** 74  
- **Orders Shipped:** 63  
- **Orders Not Shipped:** 11  
- **Not Shipped Rate:** 14.86%  

*Figure: Total Count of Orders Processed in April 2020*

---

### **2. Order Distribution by Category**
- **Top Ordered Categories:**
  - **Beverages:** 30 orders
  - **Dairy Products:** 27 orders
  - **Seafood:** 22 orders
- **Lowest Ordered Categories:** Produce (5 orders), Meat/Poultry (6 orders).

*Figure: Total Orders by Category*

---

### **3. Shipping and Non-Shipping Trends**
- Shipping patterns show most orders were shipped within the first three weeks of April.
- A small number of orders remained unshipped due to unknown reasons, distributed across multiple countries.

*Figure: Count of Orders Not Shipped by Country*

---

## Database and Data Sources

### **Primary Data Source:**
- **MariaDB Connection:**
  - Server: `relational.fit.cvut.cz`
  - Port: `3306`
  - Database: `Northwind`
  - Username: `guest`
  - Password: `relational`

### **Alternate Data Source:**
- **CSV Files:**
  - Extracted from the Northwind database.
  - Multiple CSV files were imported into MongoDB for easier handling.

### **Data Relationships:**
- **Orders**:
  - Includes Order Details, CustomerID, EmployeeID, and ShipperID (`ShipVia`).
- **Products**:
  - Linked by SupplierID and CategoryID.
- **Territories**:
  - Contains RegionID for geographic mapping.

---

## Tools and Technologies
- **Database Management:** MariaDB, MongoDB, CSV
- **Data Visualization:** Tableau
- **Programming:** Python (for data preparation and ETL workflows)
- **Dataset:** SQL's Northwind database (simplified dump into CSV)

---

## Dashboard Features
The dashboard enables the Shipping Manager to:
1. Select a specific month to analyze shipping performance.
2. View daily trends for processed, shipped, and outstanding orders.
3. Understand the geographic spread of shipping and unshipped orders.

---

## Conclusion
This project provides Amazon Trade with a robust solution to track and manage shipping operations. The dashboard's insights can enhance decision-making by:
1. Identifying delays and outstanding orders.
2. Analyzing order distribution across categories and regions.
3. Streamlining operations to improve shipping efficiency.

---

## Acknowledgments
- **Client:** Amazon Trade Shipping Manager
- **Contributors:** Data analysts and developers
- **Data Source:** Northwind database

# Dynamic Retail Dashboard (Excel)

**Project Type:** Excel Dashboard  
**Module:** Data Science Course  
**Data:** Retail (Orders, Returns, People)  
**Data Source:** Ingested from GitHub via Power Query

---

## 📌 Table of Contents
- [Project Overview](#project-overview)
- [Data Description](#data-description)
- [Data Ingestion (from GitHub)](#data-ingestion-from-github)
- [Dashboard Features](#dashboard-features)
- [Installation / Setup](#installation--setup)
- [How to Use the Dashboard](#how-to-use-the-dashboard)
- [File Structure](#file-structure)
- [Sample Data & Schema](#sample-data--schema)
- [Data Transformations](#data-transformations)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License & Contact](#license--contact)

---

## 📘 Project Overview
This project is a **dynamic retail dashboard built in Excel** as a part of my Data Science course module.  
It uses three core retail datasets:

- **Orders**
- **Returns**
- **People**

The dashboard helps analyze retail performance using Power Query, PivotTables, calculated fields, and dynamic charts.

---

## 📊 Data Description
The dataset consists of three tables loaded from GitHub using Power Query.

### **Orders Table** *(placeholder — will update once sample provided)*
Contains sales transaction details.

### **Returns Table** *(placeholder)*
Contains returned order information.

### **People Table** *(placeholder)*
Contains customer or salesperson details.

> I will update this section with exact columns once you provide sample data.

---

## 🌐 Data Ingestion (from GitHub)
Power Query steps used for ingestion:

1. Go to **Data → Get Data → From Web**
2. Paste the **raw GitHub file link**  
   Example:  
https://raw.githubusercontent.com/<username>/<repo>/<branch>/orders.csv

yaml
Copy code
3. Set correct data types in Power Query  
4. Apply transformations  
5. Load to Excel / Data Model

Raw links placeholders:

- `<GITHUB_RAW_URL_ORDERS>`
- `<GITHUB_RAW_URL_RETURNS>`
- `<GITHUB_RAW_URL_PEOPLE>`

---

## 📈 Dashboard Features
- Total Sales, Total Orders, AOV, Return Rate KPIs  
- Monthly sales trend  
- Product performance analysis  
- Region-wise sales distribution  
- Return analysis by reason  
- Interactive slicers: Date, Region, Product, Channel  
- Drill-down capability using PivotTables  

---

## 🛠 Installation / Setup
Clone the repository:
```bash
git clone https://github.com/<username>/<repo>.git
Steps:

Open Retail_Dashboard.xlsx

Enable data connections

Go to Data → Refresh All

Ensure GitHub URLs are correct in Power Query Source step

Recommended Excel Version: Office 365 / Excel 2019+

▶️ How to Use the Dashboard
Open the Excel file

Refresh queries to pull latest GitHub data

Use slicers to filter by product, date, region, etc.

View KPIs, charts, and detailed PivotTables

Navigate to raw data sheets if needed

📁 File Structure
powershell
Copy code
/ (project root)
│
├─ data/
│  ├─ orders_sample.csv
│  ├─ returns_sample.csv
│  └─ people_sample.csv
│
├─ Retail_Dashboard.xlsx
├─ README.md
└─ assets/       # screenshots, visuals
🧾 Sample Data & Schema
(Will update after you share sample rows)

Orders Sample (placeholder)
Copy code
order_id,order_date,person_id,product_id,quantity,unit_price,region,sales_channel
Returns Sample (placeholder)
Copy code
return_id,order_id,return_date,return_quantity,return_reason
People Sample (placeholder)
pgsql
Copy code
person_id,name,role,region,join_date
🔧 Data Transformations
Common Power Query transformations:

Change data types (Date, Number, Text)

Trim / clean text fields

Create calculated columns:

sales_amount = quantity * unit_price

Merge Orders ↔ People

Merge Orders ↔ Returns

Create Year / Month columns

Filter invalid or missing values

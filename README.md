# NYC Taxi Analysis Dashboard (Excel)

## 📌 Project Overview
This project analyzes NYC Yellow Taxi trip data using **Microsoft Excel** as a full analytics platform.  
The goal was to demonstrate end-to-end data analysis using **Power Query, Power Pivot, and PivotTable dashboards** following best practices used by data analysts.

The project includes:
- Data ingestion and cleaning
- Star schema data modeling
- Analytical calculations
- Interactive dashboards for insights

---

## 🗂️ Dataset
- **Source:** NYC Taxi & Limousine Commission (TLC)
- **Data Type:** Yellow Taxi Trip Records (CSV)
- **Scale:** ~41 million trips (2024)
- **Documentation:**  
  `docs/data_dictionary_trip_records_yellow.pdf`

---

## 🔧 Tools & Technologies
- Microsoft Excel
- Power Query (ETL & data cleaning)
- Power Pivot (Data Model & relationships)
- PivotTables & PivotCharts
- Slicers for interactivity

---

## 🔄 Data Preparation (Power Query)
Power Query was used to:
- Import monthly CSV files dynamically
- Combine all months into a single fact table
- Clean and standardize column types
- Create derived columns (dates, month, year)
- Prepare dimension tables

### Key Tables:
- **Fact_Trips**
- **DimVendor**
- **DimZone**
- **DimPaymentType**
- **DimRateCode**
- **DimStoreAndFwdFlag**

📸 See screenshots in `/screenshots/power_query_transformations.png`

---

## ⭐ Data Modeling (Power Pivot)
A **star schema** was created in Power Pivot:

- Dimensions connect **one-to-many** into the fact table
- Relationships flow **Dim → Fact**
- Model optimized for analytical performance

📸 See `/screenshots/data_model_power_pivot.png`

---

## 📊 Analysis & Dashboards
### Pivot Tables
A dedicated PivotTables sheet was used for:
- Revenue by vendor, payment type, rate code
- Average fare by borough
- Passenger trends by month
- Trip counts and rankings

📸 See `/screenshots/pivot_tables_sheet.png`

### Dashboard
An interactive dashboard was built featuring:
- KPI tiles (Total Revenue, Average Fare, Total Trips)
- Line charts for monthly trends
- Bar and stacked charts for comparisons
- Slicers for filtering by vendor, borough, payment type

📸 See `/screenshots/dashboard_overview.png`

---

## 🎯 Key Insights
- Credit cards account for the majority of taxi revenue
- Manhattan dominates trip volume and revenue
- Vendor performance varies significantly in trip volume vs fare averages
- Strong seasonality across months

---

## 📁 Repository Structure

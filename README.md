# 🚚 Logistics Operations Dashboard | Power BI

## 📌 Project Overview

This project presents an interactive Logistics Operations Dashboard built in Microsoft Power BI to monitor transportation performance, fleet utilization, delivery efficiency, and fuel consumption. The dashboard transforms raw logistics data into actionable insights that support operational decision-making and route optimization.

### 🎯 Objectives
Monitor overall logistics performance.
Analyze delivery success and operational efficiency.
Track fuel consumption across trips.
Evaluate vehicle and driver performance.
Identify opportunities to optimize transportation operations.


### 📊 Dataset Information

The dataset contains 50 logistics trip records with key operational attributes, including:

Trip ID
Vehicle ID
Driver ID
Origin
Destination
Distance (km)
Fuel Consumed (L)
Delivery Status
Delivery Date

The data was cleaned and prepared before visualization in Power BI.

### 📈 Dashboard Features

The dashboard provides interactive visualizations for:

Total Trips
Total Distance Travelled
Fuel Consumption Analysis
Delivery Status Distribution
Route Performance
Date-based Delivery Trends
Interactive Filters and Slicers

### DAX functions used
- To create a column that shows real fuel cost of different vehicle type based on specific locations
- Created measures for Fuel consumption, Cost per Km, Average delivery time and etc.
** Fuel Consumption = IF(ISBLANK(Trip_Data[Fuel_Consumed_L]), DIVIDE(SUM(Trip_Data[Fuel_Consumed_L]),DISTINCTCOUNT(Vehicle_Master[Vehicle_Type])),Trip_Data[Fuel_Consumed_L])
** Fuel Efficiency = DIVIDE(sum(Trip_Data[Distance_km]),SUM(Trip_Data[Fuel Consumption]))

### 🛠 Tools & Technologies
Microsoft Power BI
Power Query
DAX (Data Analysis Expressions)

### 📌 Key Insights
Identified delivery completion trends over time.
Measured fuel efficiency across transportation routes..

#### 📂 Project Files
Logistics_Dashboard.pbix – Power BI Dashboard
logistics_project_dataset.xlsx – Source Dataset

### 🚀 Skills Demonstrated
Data Cleaning
Data Transformation
Data Modelling
DAX Measures
KPI Development
Dashboard Design
Business Intelligence
Logistics Analytics
Data Visualization

📷 Dashboard Preview

!(Images)[Dashboard1.png/Images]
!(Images)[Dashboard2.png/Images]

📬 Connect With Me

If you have feedback or suggestions, feel free to connect with me on Kaggle or LinkedIn.

If you found this project useful, consider giving it an upvote on Kaggle! ⭐

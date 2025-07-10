# Smart Factory OEE & Downtime Analysis Dashboard
**1. Smart Factory Insights: Manufacturing Efficiency Dashboard**
A comprehensive Power BI dashboard solution engineered to monitor, analyze, and optimize smart manufacturing performance metrics. Designed using real-world industrial IoT data, this project provides data-driven insights into machine performance, production quality, and downtime diagnostics in a simulated smart factory environment.

**2. Project Purpose**
The Smart Factory Efficiency Dashboard leverages predictive maintenance data to uncover hidden inefficiencies, identify root causes of downtime, and drive continuous process improvement in manufacturing environments. It is tailored to assist industrial engineers, plant supervisors, and business intelligence teams in making fast, informed decisions through real-time visualization of production KPIs.

**3. Tech Stack**
This project incorporates multiple layers of modern data analytics tooling:

📊 Power BI Desktop – Core platform for interactive dashboard design and data modeling.

⚙️ Power Query (M) – Used for ETL: reshaping, cleaning, and preparing time-series and categorical data.

🧠 DAX (Data Analysis Expressions) – Custom measures and KPIs for availability, performance, and quality analysis, including dynamic OEE computation.

🧱 Data Modeling – All data fields were logically structured and relationally integrated to support drill-downs by downtime reason, torque anomalies, and machine output.

📁 .pbix File Format – The primary file used for development, easily shareable for future enhancements or stakeholder review.

**4. Data Source**
Dataset: AI4I 2020 Predictive Maintenance Dataset

Provider: UCI Machine Learning Repository

Description: Industrial data generated from simulated smart manufacturing sensors. Includes machine conditions such as torque, tool wear, process temperature, and sensor-driven binary failure flags.

Key fields include:
UDI (Unit number)
Product ID
Type
Tool wear [min]
Torque [Nm]
Rotational speed [rpm]
Process temperature [K]
Air temperature [K]
Machine failure (binary target)
Failure cause flags (TWF, HDF, PWF, OSF, RNF)

**5. Features & Analytical Highlights**
• Business Problem
Factories require high availability, efficiency, and quality—but interpreting raw sensor data and uncovering downtime drivers at scale is a challenge. Identifying machine failures early and minimizing production delays requires real-time insight into equipment behavior, failure types, and throughput quality.

• Goal of the Dashboard
To develop a modern visual interface that:
1. Provides OEE metrics using a real-world-inspired framework.
2. Allows quality engineers and BI analysts to drill into product types, sensor anomalies, and failure reasons.
3. Supports smart maintenance scheduling by surfacing patterns in torque spikes, tool wear, and rotational speed anomalies.

• Walkthrough of Key Pages & Visuals
🟦**Page 1: Factory Performance Overview**

Top KPIs (Cards):
Total Production Time
Total Productive Time
Total Downtime (min)
Overall Efficiency %
Average Production Time
Average Productive Time
Average OEE (Availability × Performance × Quality)
Sum of Machine Failure

Visuals:
📊 Bar Chart: Downtime Minutes vs Downtime Reasons and Products
📈 Line Chart: UDI vs Downtime Minutes
🔘 Gauge: OEE visualized with thresholds

🟨 **Page 2: Product Quality & Failure Insight**

Top KPIs:
Total Units
Total Good Units
Total Defective Units
Defect Rate %
Average Production Time
Top Failing Product Type
Top Downtime Product
Top Downtime Cause

Visuals:
🍩 Donut Chart:UDI by Machine Failure
📊 Bar Chart: Tool wear by UDI

🟨 **Page 3: Factors affecting Failure**

Top KPIs:
Downtime Events Count
Average Torque Failures
maximum of Air Temperature
Downtime_speed
Downtime_torque

Visuals:
📊 Clustered Column: Speed bin vs UDI
📈 Line Chart: UDI vs Torque, color-coded by Machine Failure (failure/pass)
📊 Clustered Bar Chart: Sum of UDI by Downtime Reason

**6. Business Impact & Use Cases**
Manufacturing Intelligence: Enables plant managers to quickly identify high-failure product types or machines with frequent tool wear issues.
Maintenance Optimization: Detects mechanical stress patterns based on torque and rotational speed—helping avoid unscheduled downtime.
Quality Assurance: Measures yield performance and correlates quality loss to real-time sensor inputs.
BI Strategy Alignment: The dashboard structure supports integration with broader KPIs across production lines and facilities.

🧠 Additional Enhancements
Dynamic Slicers: By Product ID, Type

Bookmarks & Navigation Toggles: User-friendly page switching between Performance and Quality views
Tooltips: Custom explanations on hover for formulas like OEE, Torque Outliers, and Defect Rate

**7. Final Deliverables**
SmartFactoryDashboard.pbix – Fully interactive Power BI file
Dashboard Screenshots (PNG) – For documentation and portfolio display


 

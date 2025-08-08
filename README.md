# Vendor-Performance-data-analytics-project
Project Overview
This is a comprehensive, company-standard data analytics project designed to optimize profitability within the retail and wholesale industry. The project focuses on analyzing vendor performance, inventory turnover, and pricing strategies to enable data-driven decision-making. Utilizing a real-world dataset, this project integrates multiple essential data skills and tools, including SQL, Python, and Power BI, to deliver a complete end-to-end analytical solution.

Business Problem
Efficient inventory and sales management are paramount for success in the retail and wholesale sectors. Businesses must actively work to prevent financial losses that can arise from inefficient pricing models, suboptimal inventory turnover rates, and an over-reliance on underperforming vendors.

This analysis is specifically structured to address the following critical business objectives:

Identify underperforming brands that necessitate targeted promotional efforts or pricing adjustments.

Determine top-tier vendors who contribute substantially to overall sales and gross profit.

Analyze the direct impact of bulk purchasing on the unit cost of products.

Assess inventory turnover efficiency to minimize holding costs and enhance operational effectiveness.

Investigate the variance in profitability observed between high-performing and low-performing vendors.

Project Workflow
The project adheres to a robust, end-to-end data analytics pipeline, mirroring real-world industry practices:

Data Ingestion and Database Setup:

Raw data, initially provided in various CSV files, is systematically ingested into a database.

SQLite is employed for this project, offering a practical solution, though the methodology is designed to be scalable for enterprise-level database systems such like PostgreSQL.

A dedicated Python script is developed, incorporating logging and well-defined functions, to automate and manage this ingestion process efficiently.

Exploratory Data Analysis (EDA) with SQL:

The raw data within the database is thoroughly explored using SQL queries.

This phase aims to deeply understand the data's structure, identify crucial columns, and map out the relationships between different tables.

The insights gained here are vital for determining which data points are most pertinent to the core business problem.

Data Aggregation and Cleaning:

Based on the findings from the EDA, a final, aggregated summary table is meticulously constructed.

This involves joining and cleaning data extracted from multiple source tables.

The consolidated table is designed to contain all necessary information for detailed analytical work, encompassing:

Vendor purchase transactions

Sales transaction data

Associated freight costs

Actual product pricing information

In-depth Analysis with Python:

The prepared aggregated data is retrieved from the database and loaded into a Jupyter Notebook.

Further iterative EDA, advanced data cleaning, and sophisticated analytical techniques are applied using Python.

The primary goal of this stage is to generate answers for the specific research questions derived from the business problem.

Interactive Dashboarding with Power BI:

Key insights, trends, and visualizations unearthed during the Python analysis are leveraged to create an intuitive and interactive Power BI dashboard.

This dashboard serves as a powerful tool, allowing stakeholders to easily comprehend and explore the project's findings.

Comprehensive Report Writing and Presentation:

A detailed, comprehensive report is prepared to document the entire project, including the methodology employed, the significant findings, and actionable recommendations.

This report is crucial for effectively presenting the analysis results to clients, management, and other key stakeholders, facilitating informed decision-making.

Data Schema
The project utilizes several interconnected tables, each holding specific transactional data. The relationships and contents of these tables were meticulously mapped during the initial exploratory data analysis phase:

begin_inventory: Contains records of inventory levels at the beginning of the reporting period (e.g., start of the year).

end_inventory: Contains records of inventory levels at the end of the reporting period (e.g., end of the year).

inventory: Provides detailed information about specific inventory items.

purchase: Stores actual purchase transaction data, including dates of purchase orders, quantities bought, and corresponding dollar amounts.

purchase_prices: Offers product-level pricing information, distinguishing between actual and vendor purchase prices.

sales: Captures actual sales transactions, detailing quantities sold, selling prices, and total revenue earned.

vendor_invoice: Aggregates summary data from purchase transactions, including additional columns like freight costs, and maintains uniqueness based on a combination of vendor and Purchase Order (PO) numbers.

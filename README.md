# Business-Insights-360-BI-Dashboard

# 📑 Project Overview
AtliQ Hardware, experiencing rapid growth in recent years, decided to adopt Power BI for the first time to strengthen its market position and drive data-informed decisions. This project was designed to address key stakeholder questions across Finance, Sales, Marketing, and Supply Chain functions through powerful analytics and reporting.

🔗 [Live Report Link](https://app.powerbi.com/reportEmbed?reportId=626566df-b997-4972-9e40-c578dc94571f&autoAuth=true&ctid=c6e549b3-5f45-4032-aae9-d4244dc5b2c4)

# 👨‍💻 Tech Stack

● SQL

● Power BI Desktop

● Excel

● DAX Language

● DAX Studio (for report optimization)

● Project Charter Documentation

# 🎓 Power BI Techniques Learned

● Key questions to ask before starting a project

● Creating calculated columns

● Building measures using DAX

● Data modeling best practices

● Implementing bookmarks for visual navigation

● Page navigation with action buttons

● Using the DIVIDE function to prevent division-by-zero errors

● Creating dynamic date tables with M Language

● Designing dynamic titles based on filters

● Using KPI indicators for performance tracking

● Applying conditional formatting with icons and background colors

● Data validation techniques for report accuracy

● Publishing reports to Power BI Service

● Setting up a Personal Gateway for automated data refresh

● Creating and managing Power BI Apps

● Collaboration, workspace management, and access control within Power BI Service

# 💼Business Related Terms

● Gross Price

● Pre-Invoice Deductions

● Post-Invoice Deductions

● Net Invoice Sale

● Gross Margin

● Net Sales

● Net Profit

● COGS - Cost Of Goods Sold

● YTD - Year to Date

● YTG - Year to Go

● Direct

● Retailer

● Distributors

● Consumer

# 🏬 Company Background
AtliQ Hardware is a fast-growing company that sells computers and accessories worldwide through three channels:

● Retailers

● Direct Sales

● Distributors

Recently, AtliQ faced unexpected losses after opening stores in America based only on surveys, intuition, and basic Excel analysis. Meanwhile, their competitors had strong analytics teams using data to make smarter decisions. To survive and succeed, AtliQ realized they must build a dedicated Analytics Team to make data-driven decisions in the future.

# 🧠 Project Kick-Off Session
Before starting the dashboard, it's important to have a clear understanding of the project by asking key questions, such as:

**❓ Important Questions Before Building the Dashboard:**

● What is the main goal of creating this Power BI dashboard?

● How will we measure the success of this project?

● What is the project deadline?

● Do stakeholders expect a preview before the final dashboard release?

● What are the stakeholders’ hopes for this project?

● What are their concerns or fears about building this dashboard?

● Who will be using the dashboard, and for what purpose?

● What are the expectations when the project is completed?

● What possible risks or problems could occur during the project?

● What data and resources are needed to build the dashboard?

● Are there any design preferences or requirements from stakeholders?

● After the kick-off meeting, the Data Engineering team provided the necessary datasets to the Analytics team for exploration and analysis.

# 🧐 Dataset Understanding
Before analyzing, it's important to understand the data structure:

Dimension Tables (Static information like customer or product details):

**dim_customer:**

● 27 markets (e.g., India, USA, Spain)

● 75 customers across all markets

● 2 platforms: Brick & Mortar (physical stores) and E-commerce (online stores)

● 3 sales channels: Retailer, Direct, Distributor

**dim_market:**

● 27 markets categorized into 7 sub-zones and 4 regions: APAC, EU, LATAM, and others.

**dim_product:**

● Divisions: P&A (Peripherals, Accessories, PC, Notebook, Desktop) and N&S (Networking, Storage)

● 14 product categories (e.g., Internal HDD, Keyboard)

● Different product variants available.

**Fact Tables (Transactional data):**

● fact_forecast_monthly:

● Forecasts customer demand in advance.

● Helps with better customer satisfaction and reduced warehouse costs.

● Data is structured monthly, showing forecasted quantities.

**fact_sales_monthly:**

● Similar to forecast table, but shows actual sales quantities.

**Other Important Tables:**

● **freight_cost:** Travel and shipping costs by market and fiscal year.

● **gross_price:** Gross price details linked with product codes.

● **manufacturing_cost:** Manufacturing cost data by product and year.

● **pre_invoice_deductions:** Discounts before invoice issuance, by customer and year.

● **post_invoice_deductions:** Additional deductions applied after invoicing.

# 📥 Importing Data into Power BI
Since the data is stored in a MySQL database, we connect Power BI to the MySQL database by providing database access credentials, and then import all the required tables for analysis.

# ✨ Data Model

● Data modeling is very important and acts as the foundation of any report. All the visuals and insights are built on top of the data model.

● If the data model is not designed properly, it can slow down the report and affect its overall performance.

● That's why it's important to follow best practices for data modeling (you can check this blog for more details).

● In this project, we used the Snowflake data modeling technique to organize the data efficiently.
![Screenshot 2025-04-28 120948](https://github.com/user-attachments/assets/1481a8c2-308f-4558-addc-3e715b8ec2e8)


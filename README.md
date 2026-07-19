🚴 AdventureWorks Sales & Returns Insights Dashboard
====================================================

An interactive Power BI report built to analyze AdventureWorks' global bike, components, clothing, and accessories business — covering sales performance, profitability, customer behavior, and product returns across six countries.

Short Description / Purpose
----------------------------

The **AdventureWorks Sales & Returns Dashboard** is a Power BI report designed to help stakeholders track revenue, profit, and order trends while monitoring product return rates across the AdventureWorks product catalog. It combines sales, returns, customer, and product data into a single model so that sales leaders, category managers, and finance teams can quickly spot performance trends, seasonality, and problem products — without digging through raw transactional data.

Tech Stack
----------

The dashboard was built using the following tools and technologies:

- **📊 Power BI Desktop** — Main data visualization and report-authoring platform.
- **📂 Power Query** — Used to clean and shape the Sales, Returns, Product, Customer, Territory, and Calendar tables before loading into the model.
- **🧠 DAX (Data Analysis Expressions)** — 40+ calculated measures covering revenue, profit, returns, targets, rolling trends, and customer-level KPIs.
- **📝 Data Modeling** — A star-schema model with a central `Sales Data` fact table and a `Returns Data` fact table, linked to `Product`, `Customer`, `Territory`, and `Calendar` dimension tables, plus a dedicated `Measure Table` and `Data Dictionary` for documentation.
- **📁 File Format** — `.pbix` for development, `.png` for dashboard preview images.

Data Source
-----------

*Source: AdventureWorks sample sales dataset (Microsoft's classic bicycle & accessories retailer dataset).*

The model covers:
- **56,046** sales transactions and **1,809** product returns
- **18,148** customer records and **293** products across **4** categories (Bikes, Components, Clothing, Accessories) and **37** subcategories
- Orders spanning **6 countries** (United States, Canada, France, Germany, Australia, United Kingdom) from **January 2020 to June 2022**

A `Data Dictionary` table is included directly in the model, listing every column across all lookup and fact tables for easy reference by anyone extending the report.

Features / Highlights
----------------------

### Business Problem
AdventureWorks sells bikes, components, clothing, and accessories across multiple countries, but sales, returns, and customer data live in separate tables. Without a consolidated view, questions like:

- Which regions and products are driving the most revenue and profit?
- How does the return rate vary by product or category?
- Are we tracking ahead of or behind revenue and profit targets?
- Who are our highest-value customers?

...are slow to answer from raw transactional tables alone.

### Goal of the Dashboard
To deliver a single interactive report that:
- Tracks total revenue, profit, orders, and customer counts at a glance
- Benchmarks current performance against rolling and month-over-month targets
- Surfaces return-rate issues by product and category before they escalate
- Lets users drill into customer-level order and revenue details

### Walkthrough of Key Visuals

- **Key KPIs**
  - Total Revenue: **₹2.49 Cr+**
  - Total Orders: **25,164**
  - Total Profit: **₹1.05 Cr+**
  - Total Customers: **17,416**
  - Overall Return Rate: **2.17%**
  - Units Sold vs. Returned: **84,174 sold / 1,828 returned**

- **Revenue & Profit Trends**
  Measures like `YTD Revenue`, `Previous Month Revenue`, `10 day rolling revenue`, and `90 days rolling profit` power trend visuals that show short- and long-term momentum alongside `Revenue Target` and `Profit target` (calculated as prior-month performance +10%).

- **Returns Analysis**
  `Return Rate`, `Bike Return Rate`, `total Returns`, and `All Returns` measures break down return performance overall and specifically for the Bikes category, helping quality and category teams flag underperforming products.

- **Order Segmentation**
  Measures such as `Bulk Order` (orders with quantity > 1), `High Ticket Orders` (orders above the average product price), `Weekend Order`, and `Red sales` (color-based segmentation) let users slice performance by order type and product attributes.

- **Customer Details View**
  A dedicated set of measures (`Total Order (customer details)`, `Total Revenue(customer details)`, `Full Name(Customer Details)`) supports a customer drill-through page for account-level analysis and average revenue per customer.

- **Price Adjustment Scenario Modeling**
  A `Price Adjustment` table combined with `Adjusted Price`, `Adjusted Revenue`, and `Adjuted Profit` measures allows what-if analysis of how pricing changes would affect revenue and profit.

### Business Impact & Insights
- **Performance Monitoring**: Leadership can track revenue and profit against rolling targets without waiting on manual reports.
- **Returns Management**: Category managers can identify high-return products/categories (e.g., Bikes) and act before returns erode margin.
- **Customer Strategy**: Sales teams can identify high-value customers using average revenue per customer and order history.
- **Pricing Strategy**: The Price Adjustment model lets finance test the revenue/profit impact of price changes before rolling them out.
- **Regional & Category Focus**: Territory and category breakdowns highlight which markets and product lines are driving the business.

Screenshots / Demos
--------------------
![**Exec dashboard**](https://github.com/arunbhadra68-Analytics/AdventureWorks-Dashboard/blob/main/EXEC%20dashboard.png)

**Map** : https://github.com/arunbhadra68-Analytics/AdventureWorks-Dashboard/blob/main/MAP.png

**Product Details** : https://github.com/arunbhadra68-Analytics/AdventureWorks-Dashboard/blob/main/Product%20Details.png

**Customer Details** : https://github.com/arunbhadra68-Analytics/AdventureWorks-Dashboard/blob/main/Customer%20Details.png

```


# 🏪 Walmart Retail Intelligence: End-to-End Sales Performance & Profit Optimization

## 📝 Project Overview
This end-to-end business intelligence project delivers a deep-dive look into macro retail metrics utilizing a high-volume Walmart sales dataset containing transactional data across multiple store departments, categories, and regions. The primary objective is to evaluate operational performance, isolate profit leaks, execute advanced Time-Intelligence tracking, and build business-ready KPIs to guide executive-level retail strategies.

The project systematically covers the full data lifecycle:
1.  **Data Cleaning & Advanced ETL** using Power Query.
2.  **Relational Data Modeling & Star Schema Architecture** to maintain optimal performance.
3.  **Dynamic DAX Formulas** for custom enterprise metrics (YoY Growth, Last Year Revenue, Target Margins).
4.  **UI/UX Dashboard Blueprinting** to create a polished, recruiter-friendly executive layout.

---

## 🛠️ Tech Stack & Tooling
*   **Data Engine:** Power Query (Data cleaning, column splitting, type standardizations, data profiling).
*   **Data Model:** Relational Star Schema (Fact and Dimension table segmentation).
*   **Language Matrix:** Data Analysis Expressions (DAX) for dynamic, complex time-intelligence filters.
*   **Visualization Suite:** Power BI Desktop (Interactive matrix reports, conditional cross-filtering, corporate UI canvas).

---

## 🚀 Step-by-Step Implementation Pipeline

### 1. 🧹 Data Engineering & Transformation (Power Query)
*   **Data Profiling:** Evaluated quality distributions, handled null values, and eliminated duplicate rows across massive transactional entries.
*   **Data Formatting:** Standardized localized date formats, synchronized currency representations, and optimized schema types to drastically decrease data model weight.
*   **Calculated Column Injection:** Structured custom index filters and conditional keys to prepare relational connections between disparate data lists.

### 2. 🗄️ Relational Data Modeling
*   **Star Schema Engineering:** Separated raw tabular datasets into high-performance structural entities containing dedicated **Fact Tables** (Transactions and Sales logs) and **Dimension Tables** (Store Locations, Categories, and Date Tables).
*   **Relationship Management:** Created strict 1-to-many relationship structures using centralized keys to prevent circular dependencies and allow lightning-fast report rendering.
*   <img width="1126" height="751" alt="wall1" src="https://github.com/user-attachments/assets/cbb439cd-37c0-461d-82b7-1338bdb19be0" />


### 3. 🧪 DAX Architecture & Business Metrics
Authored robust DAX calculations to isolate operational performance metrics. Key analytical developments include:

*   **Time-Intelligence Engineering:** Formulated advanced period-over-period tracking to compare current metrics with historical cycles:
    *   `Revenue LY = CALCULATE([Total Revenue], SAMEPERIODLASTYEAR('Date'[Date]))`
    *   `Revenue YoY % = DIVIDE([Total Revenue] - [Revenue LY], [Revenue LY], 0)`
*   **Core Aggregations:** Developed baseline enterprise metrics measuring gross transaction counts, aggregate profit pools, and moving averages across departments.
*   **Conditional Logic Frameworks:** Injected dynamic KPI indicator signals (`YoY Arrows`) utilizing UNICHAR codes to automatically update based on performance targets.

### 4. 🎨 Business Intelligence Visual Blueprint
Synthesized the back-end engineering layers into a polished, executive-level interactive visual canvas:
*   **Macro Metric Tiles:** Implemented immediate KPI indicators mapping **Total Revenue**, **Total Profit**, and **Total Volume Trends** with interactive performance coloring.
*   **Slicing Matricies:** Engineered deep-dive category break-out panels (Books, Clothing, Electronics, Home Goods, Office Supplies) featuring instant filtering toggles across Shipping Types and Target Regions.
*   **Operational Cross-Filtering:** Configured explicit visual bookmarks and selection panes, creating a smooth app-like navigation layout tailored for corporate decision-makers.

---

## 📊 Core Performance Matrix Preview
Below is the optimized core transaction metrics view embedded into the executive reporting layout:

| Category | Total Revenue | Revenue LY | Revenue YoY % | Total Profit | Profit LY | Profit YoY % | Total Transactions |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **📚 Books** | \$3,76,71,478.85 | \$3,81,25,936.98 | **-1.19%** | \$1,44,07,720.15 | \$1,45,94,407.99 | -0.01% | 27,269 |
| **👕 Clothing** | \$4,32,23,723.56 | \$4,34,19,512.68 | **-0.45%** | \$1,65,48,176.56 | \$1,66,24,553.76 | 0.00% | 31,002 |
| **⚡ Electronics** | \$4,09,18,610.83 | \$4,04,59,404.51 | **+1.13%** | \$1,56,60,616.30 | \$1,54,89,018.81 | +0.01% | 29,476 |
| **🏡 Home Goods** | \$4,07,04,963.98 | \$4,04,30,641.68 | **+0.68%** | \$1,55,82,128.27 | \$1,54,78,809.37 | +0.01% | 29,232 |
| **📎 Office Supplies** | \$3,21,58,724.11 | \$3,22,93,216.02 | **-0.42%** | \$1,23,06,917.73 | \$1,23,55,605.98 | 0.00% | 23,157 |
| **🏆 Total** | **\$19,46,77,501.33** | **\$19,47,28,711.87** | **-0.03%** | **\$7,45,05,559.02** | **\$7,45,42,395.91** | **0.00%** | **140,136** |

---

## 🖥️ Interactive Dashboard Preview

Executive Summery
<img width="1280" height="702" alt="wall" src="https://github.com/user-attachments/assets/2e068e30-f658-415e-80d8-2cff88cff7c1" />

Product & Customer Insights Dashboard
<img width="1289" height="724" alt="wall2" src="https://github.com/user-attachments/assets/5abb8719-9bf8-459b-8a9a-7d72bcf05093" />



---

## 💡 Strategic Business Insights Discovered
1.  **📈 Segmented Acceleration:** While overall macro enterprise growth stabilized flatly at **-0.03%**, the **Electronics** department represented a major growth driver, elevating gross revenue by **+1.13%** to reach **\$40.9M**.
2.  **📉 Inventory Risk Assessment:** The **Books** segment experienced the largest historical revenue decline (**-1.19% YoY**), indicating a clear need to adjust safety stock and reorder frequencies within that department block.
3.  **💡 Margin Efficiency Optimization:** Total operations successfully retained an exceptional net profit margin profile across **140,136 global transactions**, indicating strong supply chain stability despite localized revenue adjustments.

---

## ⚙️ How to Deploy & Execute Locally

### 📋 Prerequisites
*   Windows 10/11 operating system (Required for running native Power BI software desktop)
*   Power BI Desktop (Latest Edition Recommended)

### 💻 Local Verification Steps
1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/your-username/walmart-sales-analysis.git](https://github.com/your-username/walmart-sales-analysis.git)
    ```
2.  **Launch the BI Dashboard File:** Double-click `Walmart_Sales_Analysis_Report.pbix` to open the fully compiled interactive report environment.
3.  **Interact & Drill Down:** Use the filter menus, slicing panels, and category matrices to audit the live performance metrics across your screen.

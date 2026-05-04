# 🛒 Flipkart Market Analytics Dashboard

![Dashboard Preview](Screenshot%202026-05-04%20192035.png)

## 📌 Project Overview
This project is a comprehensive **Business Intelligence solution** designed to analyze Flipkart's e-commerce ecosystem. By processing a dataset of **20,000+ product listings**, I developed an interactive Power BI dashboard that uncovers critical insights into pricing strategies, brand dominance, and consumer behavior.

The goal of this analysis is to provide stakeholders with data-driven evidence to optimize discount logic and identify high-performing market segments.

## 🎯 Key Objectives
*   **Pricing Strategy:** Analyze how discounts are distributed across categories.
*   **Brand Audit:** Identify top-performing brands and those needing strategic attention.
*   **Customer Savings:** Quantify the total economic value provided to customers through discounts.
*   **Category Intelligence:** Map the product distribution across Flipkart’s vast catalog.

## 🚀 Key Business Insights
*   **Aggressive Discounting:** Approximately **43.93%** of products are listed with **High Discounts (51%+)**, indicating a strategy focused on high-volume turnover.
*   **Significant Savings:** The analysis revealed a total of **₹20 Million** in potential customer savings across the analyzed listings.
*   **Average Performance:** Maintained an average product rating of **3.98** and a platform-wide average discount rate of **40.55%**.
*   **Brand Health:** Identified brands like *Durian* as premium leaders, while pinpointing 5 specific brands (Regan, Tks, etc.) that show low revenue impact and may require re-strategizing.

## 🛠️ Technical Stack & Workflow

### 1. Data Cleaning & Preparation (Power Query)
*   Managed a dataset of **20,000+ rows** and 15 columns.
*   **Imputation:** Handled missing values for `brand` (Unknown) and used Median treatment for `retail_price` and `discounted_price`.
*   **Text Mining:** Extracted primary categories from complex `product_category_tree` strings using custom delimiter logic.

### 2. Analytical Engineering (DAX)
Developed custom measures and calculated columns to drive the dashboard's logic:
*   **Discount %:** `((Retail Price - Discounted Price) / Retail Price) * 100`
*   **Discount Segmentation:** Categorized products into `Low (0-25%)`, `Medium (26-50%)`, and `High (51%+)` buckets.
*   **KPI Metrics:** Created measures for Total Savings and Average Ratings.

### 3. Data Visualization
*   **Funnel Charts:** To visualize bottom-performing brands.
*   **Treemaps:** To show brand dominance and product listing density.
*   **Clustered Bar Charts:** For price comparison between Retail and Discounted values.

## 📂 Project Structure
```text
├── 📊 Flipkart_Dashboard.pbix               # Power BI Resource File
├── 📁 data/
│   └── flipkart_com-ecommerce_sample.csv    # Raw Dataset (Kaggle)
├── 🖼️ Screenshot 2026-05-04 192035.png     # Dashboard Preview Image
└── 📄 README.md                            # Project Documentation

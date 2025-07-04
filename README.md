# USB-and-Lightning-cable-product-analysis
![amazo-us](amazo-us.jpg)
# 📊 USB & Lightning Cables Product Analysis

## Table of Content

- [Introduction](#Introduction)
- [Project Overview](#Project-Overview)
- [Data source](#Data-source)
- [Tools used](#Tools-used)
- [Data Analysis](#Data-Analysis)
- [Visualisations](#Visualisations)
- [Key Insights](Key-Insights)
- [Recommendations](#Recommendations)
- [Conclusion](#Conclusion)

  
## 🧾 Introduction
This project focuses on analyzing Amazon product data for various USB and Lightning charging cables. The goal is to derive insights into pricing strategies, customer preferences, product performance, and user reviews to inform decision-making for manufacturers, marketers, or retailers.


## 📁 Project Overview

This analysis includes:
- Cleaning and preprocessing raw data
- Creating calculated fields
- Visualizing trends and distributions using Pivot Tables
- Deriving actionable business insights
- Making data-driven recommendations


## 🔗 Data Source

- Source: Product listing and review data were given by DSA
- Format: Structured table with fields such as:
  - `product_id`, `product_name`, `category`, `discounted_price`, `actual_price`, `discount_percentage`, `rating`, `rating_count`, `about_product`, `user_reviews`, and media/product links.

## Tools used
- Microsoft Excel
- Pivot Tables
- Calculated Columns
- Markdown for documentation

  

## 📊 Data Analysis 

### 1. 📦 Data Cleaning
- Removed blanks
- Checked for duplicate values
- Removed redundant columns
- Converted the dataset to a table

  
### 2. 📐 Calculated Columns
- `potential_revenue = actual_price * rating_count`
- `discount_bucket` → Created ranges (e.g., `<50%`, `50–69%`, `70%+`)
- `price_bucket` → Ranges like `<₹500`, `₹500–₹999`, `₹1000+`

### 3. 📈 Pivot Table Analysis

#### Q1: Average Discount % by Category
Grouped products by category and calculated average discount.

#### Q2: Product Count by Category
Counted distinct products under each product category.

#### Q3: Total Reviews per Category
Summed `rating_count` per category to identify engagement levels.

#### Q4: Products with Highest Ratings
Ranked products by `rating`, filtering for top performers.

#### Q5: Average Price Comparison by Category
Compared average `actual_price` vs `discounted_price` to evaluate pricing strategy.

#### Q6: Products with Most Reviews
Identified highly reviewed (popular) products.

#### Q7: Products with ≥50% Discount
Used conditional filter to count high-discounted items.

#### Q8: Rating Distribution
Grouped products by `rating` and counted frequency.

#### Q9: Potential Revenue by Category
Calculated potential revenue using `actual_price * rating_count`.

#### Q10: Products per Price Range
Bucketed prices into ranges to see where most products fall.

#### Q11: Correlation Between Rating and Discount
Visualized `rating` vs `discount_percentage` using scatter plot.

#### Q12: Products with <1000 Reviews
Flagged and counted low-engagement products.

#### Q13: Max Discounts by Category
Identified categories offering highest individual discounts.

#### Q14: Top 5 Products by Weighted Score
Used formula: `rating * LOG10(rating_count + 1)` to balance quality and quantity.

## Visualisations

## 🔍 Key Insights

- **Cables under ₹500 dominate** the market, especially from brands like pTron and Ambrane.
- **Discounts of 60–90%** are common and play a key role in consumer choice.
- **Rating does not strongly correlate** with discount percentage.
- Products with high ratings often come with robust reviews and warranty promises.
- Some categories consistently outperform others in both **reviews and revenue potential**.


## ✅ Recommendations

- **Bundle high-performing cables** into multipacks and promote them via review-based ads.
- **Improve documentation and product clarity** for low-rated items.
- **Invest in higher discount marketing strategies** for newer, low-reviewed products.
- **Track review quality, not just quantity**, as some reviews mention quality defects despite high counts.


## 📌 Conclusion

This project demonstrates how structured analysis of e-commerce product data can reveal powerful insights into product positioning, consumer perception, and pricing dynamics. With the help of Excel Pivot Tables and calculated columns, we were able to transform raw listing data into strategic intelligence.

### Back to top 
###### [Table of Content](#Table-of-Content)



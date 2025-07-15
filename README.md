# Amazon-product-review-analysis

This is a project given by DataSkilLUPAfrica (DSA) to analyze a dataset of Amazon-listed products using Microsoft Excel.

The goal of the analysis is to uncover insights around pricing strategy, discount effectiveness, customer reviews, and product performance. Microsoft Excel tools such as formulas, pivot tables, and charts were used to answer business questions and build a professional dashboard for decision-making.

The project simulates a role where the analyst supports RetailTech Insights, a company interested in optimizing their Amazon product listings.

## Company Overview

You are working as a **Junior Data Analyst** at **RetailTech Insights**, a company that provides **e-commerce analytics solutions** to sellers on platforms like Amazon.  
Your team has been tasked with analyzing product and customer review data to generate insights that can guide **product improvement**, **marketing strategies**, and **customer engagement**.

## Data Source !
The data was downloaded on Canvas as provided by DSA !

   ##  Dataset Description

The dataset contains information scraped from Amazon product pages, including:

- **Product details:** Name, category, price, discount, and ratings  
- **Customer engagement:** User reviews, titles, and content  
- Each row represents a **unique product**, with **aggregated reviewer data** stored as comma-separated values  

**Total Records:** 1,465 rows  
**Total Fields:** 16 columns

##  Business Task

RetailTech Insights requires a complete analysis of product reviews and pricing trends on Amazon.  
Your role is to clean and analyze the dataset to answer 14 business questions using Excel Pivot Tables and formulas, then present the insights in an interactive Excel dashboard.

The analysis will help the company:

- Identify top-rated and most-reviewed products
- Understand pricing and discount patterns across categories
- Examine how discounts relate to customer satisfaction
- Estimate potential revenue from reviewed products

##  Data Cleaning Process

To prepare the dataset for accurate analysis, the following cleaning steps were performed in Excel:

- **Removed duplicate rows** to ensure product uniqueness.
- **Handled missing values** in key fields such as `rating`, `price`, and `rating_count`.
- **Corrected column formats** for numerical fields (e.g., ensured all prices and rating counts are in number format).
- **Renamed columns** for clarity and consistency (e.g., `actual_price`, `discounted_price`, `discount_percentage`, `rating_count`).
- **Created calculated fields**:
   - `Discount %` = `(Actual Price - Discounted Price) / Actual Price * 100`
  - `Potential Revenue` = `Actual Price * Rating Count`
  - `Combined Score` = `Rating + (Rating Count / 1000)`
- **Generated bucket columns** for better analysis:
  - Price Buckets: `<₦1,000`, `₦1,001–₦5,000`, `₦5,001–₦20,000`, `>₦20,000`
  - Discount Ranges: `0–10%`, `11–20%`, ..., `81–93%`
  - Rating Levels: Rounded to nearest whole number

## 📊 Business Analysis Summary (Tasks 1–14)

1. **Average Discount % by Product Category:**  
The average discount percentage varies significantly across categories. Categories like **Home & Kitchen**, **Electronics**, and **Office Products** offer the highest discounts — often exceeding 40%. In contrast, categories such as **Books** and **Musical Instruments** offer much lower average discounts, possibly due to niche pricing or stable demand.

2. **Product Count per Category:**  
The dataset is dominated by products from **Electronics**, **Computers & Accessories**, and **Home & Kitchen**. These categories not only have the highest product counts but also offer a diverse range of items. Meanwhile, **Office Products** and **Musical Instruments** have fewer listings, which may indicate specialization or lower demand.

3. **Total Number of Reviews per Category:**  
In terms of engagement, **Home & Kitchen** and **Electronics** again take the lead, accumulating the highest total review counts. This aligns with their broad product offerings and popularity among online shoppers.

4. **Products with Highest Average Ratings:**  
Top-rated products — those with average ratings above **4.5** — appear in various categories. These products generally maintain high customer satisfaction and present strong opportunities for highlighting in ads, recommendations, or promotions.

5. **Average Actual vs Discounted Price by Category:**  
Across most categories, there is a significant drop from actual price to discounted price. This is especially visible in **Electronics**, where price reductions are aggressive. The gap highlights a common strategy of inflating actual prices to create a strong perceived discount.

6. **Products with the Highest Number of Reviews:**  
A small number of products (particularly in **Electronics** and **Home & Kitchen**) receive disproportionately high review volumes, with some exceeding **100,000 reviews**. These items are likely bestsellers and can be leveraged in featured placements or bundles.

7. **Products with ≥ 50% Discount:**  
A large number of products — nearly **30%** — are offered at **50% or more discount**, signaling heavy reliance on promotional pricing. These products may be part of clearance strategies, flash sales, or inventory push campaigns.

8. **Distribution of Product Ratings:**  
Most products fall within a rating range of **3.5 to 4.5**, with very few receiving ratings below 3. This suggests overall customer satisfaction is relatively high, and extremely poor-performing products are minimal in the dataset.

9. **Potential Revenue per Category:**  
By multiplying actual price by rating count (as a proxy for sales volume), **Electronics** emerges as the most revenue-generating category. This further supports its dominance in both pricing power and customer attention.

10. **Product Count per Price Range Bucket:**  
The largest concentration of products falls in the **₦1,001–₦5,000** price range, representing an affordable sweet spot for Amazon consumers. Very few products are priced below ₦1,000 or above ₦20,000, suggesting a middle-income pricing strategy.

11. **Relationship Between Discount and Rating:**  
When analyzing discount buckets, products with **21–60% discount** tend to receive the best average ratings. Extreme discounts (above 80%) don’t correlate with high satisfaction, and may even signal low-quality or surplus items.

12. **Products with < 1,000 Reviews:**  
Roughly **25% of products** have fewer than 1,000 reviews, showing low visibility or limited traction. These products may need more promotion, better SEO, or improved listing optimization to attract buyers.

13. **Categories with the Highest Discounts:**  
Categories like **Office Products** and **Home & Kitchen** feature the most deeply discounted products, with some reaching up to **93% off**. These may be overstocked items or part of aggressive flash sales.

14. **Top 5 Products by Rating + Reviews Combined:**  
Using a composite score of **Rating + (Review Count / 1000)**, the top 5 products identified are those that are both highly rated and heavily reviewed. These items represent the best combination of quality and popularity, ideal for hero banners or promotional bundles.

## Final Excel Dashboard

Below is a snapshot of the final interactive dashboard built in Microsoft Excel using pivot tables, slicers, and visual charts:

![Amazon Product Dashboard]()



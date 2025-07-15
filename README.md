# Amazon-product-review-analysis

This is a project given by DigitalSkilLUpAfrica (DSA) to analyze a dataset of Amazon-listed products using Microsoft Excel.

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
  - Discount Ranges: `0–10%`, `11–20%`, ..., `81–94%`
  - Rating Levels: Rounded to nearest whole number

##  Tools Used

The following tools and features were used throughout the project for data preparation, analysis, and dashboard creation:

- **Microsoft Excel**
  - **Power Query**: For data cleaning, column renaming, spliting columns and filtering null/duplicate rows.
  - **Pivot Tables**: For summarizing metrics like total reviews, average discounts, product counts, and potential revenue.
  - **Pivot Charts**: Used to visualize categories, discount buckets, ratings, and revenue.
  - **Slicers**: For interactive filtering by Category, Rating, and Price Bucket.
  - **Custom Data Labels**: Displayed in thousands (K) for better readability in charts.
    
- **Visualization Design**
  - Used a combination of KPI cards, bar charts, pie charts, and line charts
  - Maintained a consistent and minimal design for clarity and insight delivery

## Business Analysis Summary (Tasks 1–14)

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

## Charts Used in the Dashboard

The following are the visual charts used in building the Excel dashboard. Each chart was created based on the pivot table outputs and calculated columns from the cleaned dataset.

| No. | Chart Title                                       | Description                                                   | Image |
|-----|---------------------------------------------------|---------------------------------------------------------------|-------|
| 1.  | Average Discount % by Category                    | Compares the average discount percentage across categories.   | Avg Discount (<img width="670" height="250" alt="chart 9" src="https://github.com/user-attachments/assets/813e3bd2-3606-4f91-a39c-12ab230c35a3" />
) |
| 2.  | Total Reviews per Category                        | Displays the total review count for each category.            | Total Reviews (<img width="723" height="259" alt="chart8" src="https://github.com/user-attachments/assets/d106da12-2337-43e3-b701-78c94dbb3ccb" />
) |
| 3.  | Top Rated Products                                | Highlights products with the highest average ratings.         | Top Rated (<img width="716" height="269" alt="chart7" src="https://github.com/user-attachments/assets/84ba1eda-0528-4735-8129-c680da000a6d" />
) |
| 4.  | Average Actual vs Discounted Price by Category    | Compares actual vs discounted prices per category.            | Price Comparison (<img width="781" height="274" alt="chart6" src="https://github.com/user-attachments/assets/321bda5b-e135-441c-aea0-42f6601003a3" />
) |
| 5.  | Most Reviewed Products                            | Displays the top products by number of reviews.               | Most Reviewed (<img width="737" height="267" alt="chart5" src="https://github.com/user-attachments/assets/5923f856-5f86-4505-94e0-e4db0eaa4b9e" /> 
) |
| 6.  | Product Rating Distribution                       | Shows the distribution of average product ratings.            | Rating Distribution (<img width="723" height="271" alt="chart 4" src="https://github.com/user-attachments/assets/e617a645-3290-4098-9a02-ab784deccf03" />
) |
| 7.  | Potential Revenue per Category                    | Estimates revenue using actual price × rating count.          | Revenue (<img width="722" height="266" alt="chart3" src="https://github.com/user-attachments/assets/70921c28-c0d5-436b-999f-c885f17b433f" />
) |
|8.  | Product Count by Price Bucket                     | Groups products by price ranges (₦1,000–₦20,000+).            | Price Bucket (<img width="685" height="261" alt="chart2" src="https://github.com/user-attachments/assets/ea1bd82a-8425-470b-ad86-c5169fd45d0b" />
) |
| 9.  | Discount % vs Average Rating                      | Compares rating trends across discount buckets.               |  Discount vs Rating (<img width="664" height="274" alt="chart 1" src="https://github.com/user-attachments/assets/04aac33a-9e84-4413-a065-297d171f95db" />
)

## Final Excel Dashboard

Below is a snapshot of the final interactive dashboard built in Microsoft Excel using pivot tables, slicers, and visual charts:

![Amazon Product Dashboard](https://github.com/Hola-yinka/Amazon-product-review-analysis/blob/main/dashboard.PNG)

##  Amazon Product Insights Summary

Here are the top-level insights generated from analyzing 1,465 Amazon products across 16 fields:

-  **Top Categories by Popularity & Revenue:**  
  *Electronics*, *Home & Kitchen*, and *Computers & Accessories* lead in both product count and total reviews, indicating strong customer interest and high earning potential.

-  **Average Discounts Vary Widely:**  
  Discounts range from under 10% to over 90%, with **Office Products** and **Home & Kitchen** offering some of the largest markdowns.

-  **Rating Sweet Spot is 4.0 – 4.5 Stars:**  
  Most products fall in this range, showing general satisfaction. Extreme discounts (>80%) do not always lead to better ratings.

-  **Mid-Priced Products Dominate:**  
  The majority of products are priced between **₦1,001 and ₦5,000**, suggesting affordability is key for this audience.

-  **25% of Products Are Under-Reviewed (<1,000 Reviews):**  
  These products lack visibility and might benefit from improved SEO, marketing, or better positioning.

-  **Top 5 Products (High Rating + High Reviews):**  
  These standout items are ideal for banner placements, bundling, or upselling due to their proven popularity and performance.

-  **Best Performing Discount Buckets:**  
  Products with **21–60% discounts** strike the best balance between attractiveness and customer satisfaction.

##  Contact

Prepared and documented by **Olayinka Ogunmilade**
- 📧 Email: Ogunmiladeolayinka122@gmail.com  
- 💼 LinkedIn: [linkedin.com/in/olayinka](https://www.linkedin.com/in/olayinka-ogunmilade/)  
Feel free to connect, collaborate, or reach out for any questions or feedback.



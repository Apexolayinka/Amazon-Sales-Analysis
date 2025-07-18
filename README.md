# Amazon-Sales-Analysis
This is a project analysis on data culled from Amazon sales 
## Project Topic: Amazon Sales Analysis
## Aim of this Project
This project aims to analyse Amazon product reviews using Excel to unravel tangible insights into the product sales, by answering some questions, thereby providing improvement in the sales, strategies and marketing, those are as follows:
  - - Average discount by category
  - - Number of products per category
  - - Total reviews by category
  - - Top-rated products
  - - Average actual vs discount price
  - - Most-reviewed products
  - - Products with ≥50% discount
  - - Rating distribution
  - - Potential Revenue
  - - Product count per price range
  - - Rating vs discount trebd
  - - Products with less than 1000 reviews
  - - Categories with the highest discounts
   - - Top 5 products (rating + review count)
## Tools Used
Excel: Used excel to carry out the following: formulas, conditional formtting, pivot table and pivot charts.
Data Cleaning Summary
To maintain the integrity of the source data, all cleaning was done on a copy of the original dataset. The following steps were carried out:
Duplicate Removal: Based on the unique Product ID, 114 duplicate rows were removed leaving 1,351 unique products.
Fields Reduction: Fields not needed for the analysis were deleted to streamline the dataset.
Data Type Consistency: Each column was checked and formatted correctly (numbers, general, accounting).
Missing and Inaccurate Values: Two blank values in the 'Rating Count' column were replaced with 0, rather than deleted because it was noted that such replacement would not impact the analysis as significantly as total row deleting would. Also, a non-numeric character "/" in the 'Rating' column was replaced with 0 and interpreted as N/A during analysis.
Category Cleanup (Power Query): The 'Product Category' field was cleaned and restructured to isolate parent categories. Used Power Query's Split Column, Replace Values, and Text.Trim to format and remove subcategories.
New Fields Created:

Sort Order column
Price and Discount Range Buckets
Rating Score combining rating and review count
Analysis
Calculated Columns & Formulas
Rounded Rating: Used 'MROUND' to round ratings to the nearest 0.5 to achieve a more defined rating range.

Potential Revenue: Calculated as 'Actual Price x Rating Count' with a total of ₹113+ billion.

Discount %: Recalculated using the products actual prices vs discount prices to ensure maximum accuracy of data.

Bucketed Data: Used

'=VLOOKUP' for price and discount grouping.
'=COUNTIF' to identify products with ≥50% discount (660) and less than 1000 reviews (307).
Rating Scores: Comined rating and number of reviews to rank products
Pivot Tables
To answer the business questions, various pivot tables were created to group and summarize the data. These tables allowed for quick aggregation and comparison across product categories, price ranges, discount levels, and customer engagement metrics.

Anlaysis Interpretation
Top-Rated Products: Products in the Computer & Accessories category dominate the list, with three achieving a perfect 5.0 rating.
Most Reviewed Product: 'Amazon Basics Flexible HDMI Cable' (Product ID: 'B07KSMBL2H'), Electronics Category is the most reviewed product with a total review of 426,973.
Top Products by Rating Score: Top 5 products all came from Electronics, based on a comnibed score factoring rating and number of reviews.
Highest Discounted Product Category: Computer & Accessories have the highest discount of 94.12%, followed closely by Electronics with 91% discount.
Price Range With Most Product: Products sold for <₹1000 has the most products of 738 products.
Category With the Highest Potential Revenue: Electronics has the highest Potential revenue of over ₹91+ Billion.
Most Rating: 789 products has an average rating of 4.0 (ranging from 3.8 - 4.2)
Most Reviewed Category: Electronics is the most reviewed category with a total of 14,208,406 reviews.
Category With the Highest Number of Products: Electronics with 490 products has the highest number of products.
Category With the Highest Average %Discount: Home Improvement with 57.94% discount has the highest average % discount.
Relationship Between Average Rating and %Discount: There's a slight downward trend in average rating as discount percentages increase. While the change is not dramatic (4.2 to 4.0), it may indicate that heavily discounted products receive slightly lower customer satisfaction — possibly due to quality perceptions or product performance. This trend suggests that discounting should be used strategically rather than broadly. However, the %Discount Bucket with the highest rate has just 1 product in it.
Visualizations
Charts
The dataset was visualized using a variety of charts:
Bar Charts
Clustered Columns
Line Chart
Dashoard
A dashboard was designed in Excel incorporating the charts above, along with slicers and KPI cards for interactivity. View Dashboard,








Conclusion
The key findings of the analysis reveals that:
High-performing products, in terms of both ratings and review volume, are concentrated in specific categories, most notably Electronics, highlighting opportunities for focused investment and targeted promotion.
While discounts are widely used, steep discounts do not correlate with higher ratings, suggesting sellers should be cautious about associating aggressive price cuts with improved customer satisfaction.
Category like 'Home Improvement' offers the deepest discounts, yet do not lead in customer engagement metrics, indicating a potential misalignment between pricing and perceived value.
Most customers rate products in the 4.0 range, suggesting a competitive baseline, while less than 25% of products fall below 1,000 reviews, providing a benchmark for customer engagement.
Revenue insights show that a small subset of products and categories drive the majority of potential revenue, emphasizing the importance of identifying and supporting top-performing listings.
 





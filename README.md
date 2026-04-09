# Power BI Case Study 
### From Raw Data to Market Insights in Residential Real Estate

---
# Shelby County Home Sales Analysis (Power BI)

## Overview

This project analyzes residential home sales data in Shelby County, TN using Power BI. The goal was to understand how pricing impacts days on market and identify trends across ZIP codes.

A key focus of this project was identifying and resolving a data visualization issue that impacted the accuracy of insights.

---

## Live Case Study

View the full project:
👉🏾 https://lajordan09.github.io/powerbi-case-study/

---

## The Problem

While building a scatter plot to analyze pricing vs. days on market, the visualization did not display correctly:

* Data points were clustered and unclear
* The distribution did not reflect expected market behavior
* Multiple points appeared for the same ZIP code

This made the analysis difficult to interpret and unreliable.

---

## Root Cause

The issue was caused by a combination of:

* Row-level data being used instead of aggregated data
* Inconsistent ZIP code formatting (ZIP+extra values)
* Power BI grouping data incorrectly due to data structure

---

## Solution

To fix the issue, I:

* Cleaned ZIP codes using Power Query (removed suffix values)

* Created a summarized table grouped by ZIP code

* Calculated:

  * Average List Price
  * Average Days on Market
  * Total Transactions

* Rebuilt the scatter plot using aggregated data to ensure one data point per ZIP

---

## Outcome

The updated visualization:

* Clearly shows the relationship between price and time on market
* Provides accurate, ZIP-level insights
* Improves usability for real estate decision-making

---

## Key Takeaways

* Data structure directly impacts visualization accuracy
* Aggregation must align with the level of analysis
* Cleaning categorical fields (like ZIP codes) is critical
* Debugging visuals is as important as building them

---

## Tools Used

* Power BI
* Power Query
* DAX
* Excel

---

## Project Structure

* index.html (case study page)
* before.png / after.png (visual comparison)
* Data cleaning and transformation steps

---

This project builds on a prior SQL analysis where the dataset was extracted, cleaned, and explored:

👉🏾 https://github.com/lajordan09/shelby-county-home-sales-analysis-

The Power BI dashboard extends that work by transforming the data into a visual, decision-support tool.

---

## Next Steps

* Create Workflow for Report Type
* Add query to workflow to clean Zip field
* Add time-based trends (monthly/quarterly analysis)
* Expand dataset with additional variables
* Build a multi-page dashboard

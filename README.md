# Zomato Exploratory Data Analysis

An exploratory analysis of a supplied Zomato restaurant dataset using Python. The project examines restaurant categories, customer votes, ratings, online ordering, table booking, and approximate cost for two people.

## Project Overview

The analysis uses restaurant-level records to summarize the dataset, check data quality, compare restaurant types, and explore how ratings relate to votes and online-order availability.

## Objectives

- Inspect the dataset structure and summary statistics.
- Prepare ratings and column names for analysis.
- Check for missing values and duplicate records.
- Compare restaurant types by votes, count, average rating, and approximate cost.
- Explore ratings against votes and online-order availability.

## Tools

Python, Jupyter Notebook, Pandas, NumPy, Matplotlib, and Seaborn.

## Dataset

The supplied CSV contains 148 records and 7 columns.

| Field | Description |
| --- | --- |
| Restaurant Name | Restaurant name |
| Online_Order | Online-order availability |
| Book_Table | Table-booking availability |
| Rate | Rating in `x/5` format |
| Votes | Number of customer votes |
| Approx_Cost(For Two People) | Approximate cost for two people |
| Listed_In(Type) | Restaurant category |

## Data Cleaning

- Converted ratings such as `4.1/5` to numeric values.
- Lowercased column names and renamed the cost column to `approx_cost`.
- Checked for missing values and duplicate rows; none were found.

## EDA Questions

1. How many customer votes has each restaurant type received?
2. How many restaurants offer table booking?
3. Which five restaurant records have the highest number of votes?
4. Is there a relationship between restaurant ratings and customer votes?
5. What is the average rating for each restaurant type?
6. Which restaurant type is most common in the dataset?
7. What ratings do restaurants most commonly receive?
8. Which restaurant type has the highest average cost for two people?
9. Do restaurants offering online ordering have higher ratings?
10. Which restaurant types have more records without online ordering?

## Key Findings

- Dining is the largest category, with 110 of 148 records (74.3%), and has the most votes (20,363).
- Table booking is available in 8 records (5.4%); 140 records (94.6%) do not offer it.
- Empire Restaurant has the highest vote count (4,884), followed by Meghana Foods (4,401). Onesta appears twice among the top five records.
- Ratings and votes have a moderate positive correlation of approximately 0.49; this does not imply causation.
- The `other` category has the highest mean rating (3.91). Overall, the mean rating is 3.63, the median is 3.7, and the mode is 3.8.
- Buffet has the highest mean approximate cost for two (671.43). The report does not specify a currency.
- Records with online ordering average 3.86, compared with 3.49 for records without it. Dining has the most records without online ordering (77).

## Conclusion

Dining is the most common category and has the highest total votes. Buffet has the highest average approximate cost, while `other` has the highest mean rating. Online-order availability is associated with higher ratings in this sample. These results describe the 148 supplied records and should not be generalized to all Zomato restaurants.
## Author Anand Bhujbal

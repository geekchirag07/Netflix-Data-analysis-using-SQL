# 🎬 Netflix Data Analysis Using SQL

## Project Overview

This project analyzes the Netflix titles dataset using SQL to answer **15 business questions** about the platform's movies and TV shows. The queries explore content distribution, ratings, release years, countries, genres, directors, actors, duration, and descriptions.

The project demonstrates how SQL can be used to transform a raw dataset into useful summaries and answer practical analytical questions.

## Objectives

- Compare the number of Movies and TV Shows.
- Identify the most common content rating for each type.
- Retrieve titles released in a selected year.
- Find countries with the highest number of titles.
- Identify the longest movie.
- Find titles added within the last five years.
- Search for titles associated with a specific director.
- Find TV shows with more than five seasons.
- Count content items by genre.
- Analyze Netflix titles from India by release year.
- Retrieve documentary movies.
- Identify records with missing director information.
- Search for movies featuring a selected actor within a recent release-year window.
- Find actors appearing most frequently in Indian content.
- Categorize descriptions based on the presence of the words “kill” or “violence”.

## Tools & Technologies

- **PostgreSQL** — SQL querying and analysis
- **SQL** — filtering, grouping, aggregation, sorting, subqueries, CTEs, window functions, string functions, date functions, and `CASE` expressions
- **CSV** — source dataset format

> The supplied SQL uses PostgreSQL-specific syntax, including `UNNEST`, `STRING_TO_ARRAY`, `SPLIT_PART`, `ILIKE`, `TO_DATE`, and `::` type casting.

## Dataset

**File:** `netflix_titles.csv`  
**Rows:** 8,807 titles  
**Columns:** 12

The dataset contains the following fields:

| Column | Description |
|---|---|
| `show_id` | Unique title identifier |
| `type` | Movie or TV Show |
| `title` | Title name |
| `director` | Director or directors |
| `cast` | Cast members |
| `country` | Country or countries associated with the title |
| `date_added` | Date the title was added to Netflix |
| `release_year` | Original release year |
| `rating` | Content rating |
| `duration` | Movie duration or TV-show season count |
| `listed_in` | Genre/category labels |
| `description` | Short content description |

The dataset has **6,131 Movies** and **2,676 TV Shows**. The `release_year` values range from 1925 to 2021. Several columns contain missing values, particularly `director`, `cast`, and `country`.

## Business Questions & SQL Concepts

| # | Business question | SQL concepts demonstrated |
|---:|---|---|
| 1 | How many Movies and TV Shows are listed? | `GROUP BY`, `COUNT` |
| 2 | What is the most common rating for Movies and TV Shows? | CTEs, aggregation, `RANK()` |
| 3 | Which titles were released in a specific year, such as 2020? | `WHERE` filtering |
| 4 | Which five countries have the most content? | `STRING_TO_ARRAY`, `UNNEST`, aggregation, sorting, `LIMIT` |
| 5 | What is the longest movie? | Filtering, string parsing, type casting, sorting |
| 6 | Which titles were added in the last five years? | Date conversion, date arithmetic |
| 7 | Which titles are associated with director Rajiv Chilaka? | String splitting, subquery, filtering |
| 8 | Which TV shows have more than five seasons? | Filtering, string parsing, type casting |
| 9 | How many titles are listed under each genre? | `UNNEST`, aggregation |
| 10 | Which release years have the highest share of Indian titles? | Filtering, grouping, subquery, percentage calculation |
| 11 | Which movies are documentaries? | `LIKE` pattern matching |
| 12 | Which titles have no director listed? | `IS NULL` |
| 13 | Which movies featuring Salman Khan were released in the last ten years? | Pattern matching, date/year filtering |
| 14 | Which actors appear most often in Indian content? | String splitting, aggregation, sorting, `LIMIT` |
| 15 | How many titles fall into “Good” or “Bad” description categories based on keywords? | `CASE`, `ILIKE`, subquery, grouping |

## SQL Skills Demonstrated

- Data exploration and aggregation with `COUNT()` and `GROUP BY`
- Filtering records with `WHERE`, `LIKE`, `ILIKE`, and `IS NULL`
- Sorting and limiting results with `ORDER BY` and `LIMIT`
- Common Table Expressions (CTEs)
- Window functions such as `RANK()`
- Subqueries and nested queries
- Parsing comma-separated values with `STRING_TO_ARRAY()` and `UNNEST()`
- Working with dates and intervals
- Converting text values to numeric values
- Calculating percentages
- Conditional classification using `CASE`



## Conclusion

The Netflix Data Analysis project demonstrates practical SQL skills through 15 business-oriented questions on a real-world entertainment catalogue dataset. It is suitable for showcasing SQL querying, data exploration, aggregation, string manipulation, date handling, and analytical problem-solving in a data analyst portfolio.

---

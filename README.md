# Video Game Sales and Engagement Analysis

## Project Overview

This project analyzes and visualizes video game sales and engagement data to uncover trends in game popularity, user behavior, and platform performance. By merging sales and engagement data, the goal is to support data-driven decision-making for developers, marketers, and publishers.

## Objectives

- Structure and clean raw data using SQL.
- Merge game engagement and global sales datasets.
- Develop interactive Power BI dashboards.
- Derive insights on genre success, platform trends, and user engagement.

## Datasets

### 1. `games.csv` (Game Engagement Data)
Contains metadata and user engagement metrics:
- `Title`
- `Rating` (user review score)
- `Genres` (may include multiple categories)
- `Plays`
- `Backlogs`
- `Wishlist`
- `Release Date`
- `Platform`
- `Team` (developer name)

### 2. `vgsales.csv` (Sales Data)
Includes global and regional video game sales:
- `Name`
- `Platform`
- `Year`
- `Genre`
- `Publisher`
- `NA_Sales`, `EU_Sales`, `JP_Sales`, `Other_Sales`, `Global_Sales`

## Business Use Cases

### Game Marketing Strategy
- Identify high-performing genres and platforms.
- Analyze rating and wishlist trends to understand user preferences.

### Product Development
- Evaluate how game attributes (e.g., genre, rating, developer) relate to success.
- Determine key features driving user engagement and sales.

### Sales Forecasting
- Forecast future game demand based on historical performance.
- Measure the impact of ratings and wishlists on sales trends.

### Resource Allocation
- Prioritize development on commercially successful platforms and genres.
- Identify underserved markets and high-opportunity regions.

## Methodology

### 1. Data Cleaning
- Remove duplicates and handle null values.
- Normalize categorical fields (e.g., genre, platform, publisher).
- Standardize dates and formats.

### 2. SQL Database Design
- Create structured tables for metadata, sales, and merged datasets.
- Implement primary and foreign keys to maintain referential integrity.

### 3. Power BI Integration
- Connect Power BI to the SQL database.
- Build relationships across tables.
- Create dashboards with slicers, filters, drilldowns, and KPI cards.

### 4. Data Visualization
- Bar charts: Top genres, publishers, and platforms.
- Heatmaps: Regional genre sales.
- Line charts: Sales and wishlist trends over time.
- Scatter plots: Ratings vs. sales or wishlist count.
- KPI indicators: Total plays, average ratings, top combinations.

### 5. Exploratory Data Analysis (EDA)
- Analyze trends in ratings, plays, and wishlists.
- Explore platform and genre popularity.
- Identify drivers of successful game launches.

## Analytical Questions Answered

### From `games.csv`
- What are the top-rated games by user reviews?
- Which developers have the highest average ratings?
- What are the most common genres?
- Which games have the highest backlog-to-wishlist ratio?
- What is the trend of game releases across years?
- What is the distribution of user ratings?
- What are the top 10 most wishlisted games?
- What’s the average number of plays per genre?
- Which studios are the most productive and impactful?

### From `vgsales.csv`
- Which region generates the most game sales?
- What are the best-selling platforms?
- What is the trend of game releases and sales over years?
- Who are the top publishers by sales?
- Which games are the top 10 best-sellers globally?
- How do regional sales compare for specific platforms?
- How has the market evolved by platform over time?
- What are the regional genre preferences?
- What’s the yearly sales change per region?
- What is the average sales per publisher?
- What are the top 5 best-selling games per platform?

### From Merged Dataset
- Which game genres generate the most global sales?
- How does user rating affect global sales?
- Which platforms have the most games with high ratings?
- What is the trend of releases and sales over time?
- Do highly wishlisted games lead to more sales?
- Which genres have high engagement but low sales?
- Is there a correlation between wishlist/backlog volume and ratings?
- How does user engagement differ across genres?
- What are the top-performing combinations of genre and platform?
- What does a regional sales heatmap by genre reveal?

## Results

- A cleaned and structured SQL database integrating engagement and sales data.
- Power BI dashboards with interactive charts and KPIs.
- Insightful visualizations on user preferences, platform success, and sales trends.
- Clear recommendations for marketing, development, and publishing strategies.

## Tools Used

- SQL (PostgreSQL / MySQL / SQLite)
- Power BI
- Excel / CSV for raw data
- Python (optional, for additional EDA and preprocessing)

## Getting Started

To reproduce the project:
1. Import both datasets (`games.csv` and `vgsales.csv`) into a SQL database.
2. Clean and normalize the data using SQL scripts.
3. Establish table relationships (via keys like `Game Title` and `Platform`).
4. Connect Power BI to the database.
5. Build and customize the dashboard using the report queries.

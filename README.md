# Netflix Shows and Movies - SQL Database Project
![](logo.png)

## Overview
This project involves a comprehensive analysis of Netflix's movies and TV shows data using SQL. The goal is to extract valuable insights and answer various business questions based on the dataset. The following README provides a detailed account of the project's objectives, business problems, solutions, findings, and conclusions.
The purpose of this project is to demonstrate data normalization and SQL database creation skills, transforming a flat CSV file into a structured and normalized SQL database.

## Database Structure
The database consists of multiple tables, each representing a specific aspect of the Netflix dataset. The tables are normalized to reduce redundancy and improve data integrity. The final table, `ALL_SHOW_INFO`, combines data from all these tables to provide a comprehensive overview of the dataset.

### Tables in the Database:
- `MOVIES`: Contains movie titles and their IDs.
- `DIRECTOR`: Stores director names and their IDs.
- `CAST`: Lists cast members and their IDs.
- `MISC`: Includes miscellaneous information like country and type.
- `TIME_INFO`: Contains time-related data such as date added and release year.
- `RATING`: Stores rating descriptions and their IDs.
- `LISTED_IN`: Lists genres/categories and their IDs.
- `MOVIE_DESCRIPTIONS`: Provides descriptions of shows and movies.
- `MOVIE_INFO`: Contains additional movie information like duration.
- `DATA_RATING`: Links shows to their ratings.
- `DATA_LISTED_IN`: Links shows to their genres/categories.
- `CASTING`: Connects shows to their directors and cast members.

The `ALL_SHOW_INFO` table is a comprehensive table that combines data from all the above tables using SQL joins. It includes fields like show ID, title, director name, cast members, country, date added, release year, rating description, duration, genre, description, and type.

## Usage Instructions
1. **ALL_TOGETHER.sql**: Run this file first to create the entire database with all the individual tables.
2. **final_TABLE.sql**: Execute this file to create the `ALL_SHOW_INFO` table, which consolidates all fields into a single table.
3. **Database_queries.sql**: This file contains queries to display the top 100 rows from the `ALL_SHOW_INFO` table. Running these queries will showcase that the database and the final table have been set up correctly.

This README is intended to provide a comprehensive guide to understanding and navigating the database created from the Netflix dataset. Each step is crucial for the proper setup and viewing of the data within the SQL environment.

The Entity-Relationship Diagram (ERD) below visually represents the structure and interconnections of the various tables within the database. This diagram illustrates how data is organized and related across different aspects of the Netflix shows and movies dataset. (Once I have time I will combine several tables into one such as a single MOVIES table which would contain show_id, title, description, duration, etc.)  
  
<img width="1728" alt="image" src="Schema.png">  
  
## Potential Business Questions

### 1. Retrieve the top 5 most popular movies based on their number of cast members
📌 Business Objective:
Identify movies with the largest cast to understand production scale, star power, and potential audience appeal. Useful for marketing and content promotion.

![](Outputs/5_most_popular_movies.png)

### 2. Find the number of movies released per year
📌 Business Objective:
Analyze movie production trends over time to determine industry growth, peak production years, and shifts in content creation.

![](Outputs/movies_released_per_year.png)

### 3. Get movies that belong to multiple genres
📌 Business Objective:
Identify versatile movies that appeal to diverse audiences. Useful for content recommendation systems and genre-based promotions.

![](Outputs/Directors_in_multiple_genres.png)

### 4. List all movies along with their director
📌 Business Objective:
Provide insights into director-movie relationships for industry research, fan engagement, and content navigation on streaming platforms.

![](Outputs/Movies_with_their_directors.png)

### 5. Find the top 5 most frequent directors
📌 Business Objective:
Identify the most prolific directors, helping in talent acquisition, industry analysis, and promotional collaborations.

![](Outputs/most_frequent_directors.png)

### 6. Get the number of movies per genre
📌 Business Objective:
Understand genre popularity to guide content acquisition, platform recommendations, and audience targeting.

![](Outputs/Movies_per_genres.png)

### 7. Retrieve movies with a specific rating (e.g., 'PG-13')
📌 Business Objective:
Enable filtering based on audience age suitability, ensuring appropriate content recommendations and regulatory compliance.

![](Outputs/Movies_with_PG-13.png)

### 8. Find the longest movie duration in each genre
📌 Business Objective:
Analyze movie length trends across genres to optimize user engagement strategies and streaming platform recommendations.

![](Outputs/Longest_duration_Movies.png)

### 9. Find the total number of movies per country
📌 Business Objective:
Identify key movie-producing countries for international market expansion, content acquisition, and regional licensing deals.

![](Outputs/total_movies_per_country.png)

### 10. Get the most common movie duration
📌 Business Objective:
Understand standard movie lengths to align content strategies with audience viewing preferences.

![](Outputs/Most_common_movie_duration.png)

### 11. Retrieve all directors who have worked in multiple genres
📌 Business Objective:
Identify versatile directors for diverse content creation, talent hiring, and cross-genre collaborations.

![](Outputs/Directors_in_multiple_genres.png)

### 12. Find the top 2 countries producing the most movies
📌 Business Objective:
Determine dominant movie-producing countries to guide investment, partnerships, and content licensing strategies.

![](Outputs/most_movies_Producing_country)

### 13. Retrieve the shortest movie in the dataset
📌 Business Objective:
Understand content variations in runtime, useful for categorizing short films, optimizing platform recommendations, and audience engagement.

![](Outputs/Shortest_movie.png)


These queries leverage the rich data available in this Netflix shows and movies database to guide decision-making in content strategy, marketing, production, and more.

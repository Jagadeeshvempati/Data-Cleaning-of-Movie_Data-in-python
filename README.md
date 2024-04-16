# Data-Cleaning-of-Movie_Data-in-python

Description of the provided code:


Suppress Warnings: The code starts by suppressing warnings to enhance readability.


Import Libraries: Necessary libraries such as NumPy and Pandas are imported.


Read Data: Data is read from a CSV file named 'movie_data.csv' into a Pandas DataFrame named 'movies'.


Data Cleaning:

Columns with a high proportion of missing values are dropped.
Rows with missing values in the 'gross' and 'budget' columns are removed.
Rows with fewer than five missing values are retained.
Missing values in the 'language' column are filled with 'English'.


Data Transformation:

Currency columns ('gross' and 'budget') are converted from dollars to millions of dollars.
A new column 'profit' is created by subtracting 'budget' from 'gross'.

Data Analysis:

Movies are sorted by 'profit' in descending order.
Top 10 profitable movies are selected.
Duplicate rows are dropped from the DataFrame.
Top 10 movies are selected again after removing duplicates.
Movies are sorted by IMDb score, and only those with more than 25,000 votes are considered.
The top 250 movies are selected and ranked based on IMDb score.
Non-English language films are filtered out.
Top 10 directors based on IMDb score are identified.
The 'genres' column is split into two new columns ('genre_1' and 'genre_2').
The DataFrame is grouped by genre combinations.
The five most popular genre combinations based on mean gross are identified.
Separate DataFrames for movies featuring Meryl Streep, Leonardo DiCaprio, and Brad Pitt in lead roles are created.
These DataFrames are combined.
Statistics such as mean user reviews and mean critic reviews are calculated for each actor.

Quality Check: Null values are checked in the combined DataFrame 'Combined'.

Summary Statistics: Mean user reviews and mean critic reviews are calculated for each actor.

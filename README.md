# Movie-Popularity-Analysis
# What Makes a Movie Popular?

## Analyzing the Relationship Between Genre, Runtime, Ratings, and Audience Interest

## Overview

What makes a movie popular?

This project uses IMDb movie data to explore the relationship between movie ratings, audience interest, genre, runtime, and release period.

The goal is to identify patterns in the types of movies that receive high ratings and strong audience engagement, while also examining how these patterns have changed over time.

## Research Questions

This project investigates the following questions:

1. Is there a relationship between a movie's IMDb rating and the number of audience votes it receives?
2. Which movie genres receive the most audience interest?
3. Which genres have the highest average IMDb ratings?
4. Has the average runtime of movies changed over time?
5. Which decades produced the highest-rated movies?
6. Do highly rated movies necessarily receive a large number of audience votes?

## Dataset

The data comes from the **IMDb Non-Commercial Datasets**.

Two datasets were used:

* `title.basics.tsv.gz` — movie titles, release years, runtime, and genres
* `title.ratings.tsv` — IMDb ratings and number of votes

The datasets were joined using IMDb's unique title identifier, `tconst`.

The analysis was limited to titles classified by IMDb as movies.

## Methodology

The analysis was conducted using Python and included:

* Loading and combining IMDb datasets
* Filtering the data to movie titles
* Cleaning missing values and converting numerical fields to appropriate data types
* Exploring movie ratings and audience votes
* Separating movies into individual genres for genre-level analysis
* Examining average movie runtime over time
* Comparing average ratings across decades
* Analyzing movies with at least 1,000 IMDb votes as a measure of more widely engaged titles

## Tools Used

* **Python**
* **Pandas** — data cleaning and analysis
* **NumPy** — numerical calculations
* **Matplotlib** — data visualization
* **Google Colab** — development environment
* **GitHub** — project documentation and portfolio presentation

## Key Findings

The final findings from the analysis are presented in the accompanying `MovieA.ipynb` notebook.

The analysis focuses on:

* The relationship between IMDb ratings and audience votes
* Differences in audience interest across genres
* Differences in average ratings across genres
* Changes in movie runtime over time
* Rating patterns across different decades
* Whether highly rated movies also tend to receive substantial audience engagement

## Limitations

There are several limitations to this analysis:

* IMDb ratings are based on user-submitted ratings and may not represent the opinions of the entire movie-viewing population.
* The number of IMDb votes is a measure of audience engagement on IMDb, not total movie viewership.
* Older movies may have different levels of audience exposure and voting activity compared with newer movies.
* Movies can belong to multiple genres, so a single movie may contribute to multiple genre-level calculations.
* Some movies have missing information such as runtime, genre, or release year.
* Relationships identified in the analysis should not automatically be interpreted as causal relationships.

## Project Files

* [`MovieA.ipynb`](MovieA.ipynb) — complete analysis notebook

## Data Source

IMDb datasets:

https://developer.imdb.com/non-commercial-datasets/

The raw IMDb datasets are not included in this repository because of their size. The notebook was developed using the IMDb datasets described above.

## How to Run the Project

1. Download the IMDb datasets from the official IMDb dataset source.
2. Open `MovieA.ipynb` using Google Colab or Jupyter Notebook.
3. Upload the required IMDb dataset files to the notebook environment.
4. Run the notebook cells in order.

## Conclusion

This project demonstrates how Python and data analysis can be used to investigate patterns in movie popularity and audience engagement.

Rather than defining popularity using a single metric, the analysis considers multiple factors including ratings, number of votes, genre, runtime, and release period.

The results provide a starting point for understanding how audience interest and movie ratings vary across different types of films and periods of time.

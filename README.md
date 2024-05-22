# data-sourcing-challenge aka Movie Review Data Preparation for Recommendation System

## Background
The task involves preparing data for a recommendation system that aids users in discovering movie reviews and related films. Data will be sourced from The New York Times API and The Movie Database, merged, and later utilized for natural language processing.

## Files
- Module 6 Challenge files.

## Setup
- Create a repository named `data-sourcing-challenge`.
- Clone the repository.
- Add `retrieve_movie_data.ipynb` and `.env` (previously `example.env`) with API keys to the local repository.
- Push changes to GitHub or GitLab.

## Instructions
Complete the challenge in three parts:

### Part 1: Access the New York Times API
- Construct `query_url` using provided variables.
- Create `reviews_list` to store API responses.
- Loop through 20 pages to retrieve reviews, handling rate limits with a 12-second interval.
- Use `json.dumps` to preview results.
- Convert `reviews_list` to a DataFrame.
- Extract movie titles and convert "keywords" column to strings.
- Generate a list of titles for querying The Movie Database.

### Part 2: Access The Movie Database API
- Build query URLs for searching by title and retrieving movie details.
- Create `tmdb_movies_list` to store API responses.
- Iterate through titles, making GET requests to search and retrieve movie details.
- Extract genres, languages, and production countries.
- Append movie details to `tmdb_movies_list`.
- Preview results and convert to DataFrame `tmdb_df`.

### Part 3: Merge and Clean the Data for Export
- Merge DataFrames on the title column.
- Clean list columns and remove unwanted characters.
- Drop duplicates and reset index.
- Export cleaned data to CSV.

## Hints and Considerations
- Review Python and Pandas lessons for refresher on actions.
- Use pseudocode to outline the process.
- Debug incrementally to ensure code sections run correctly.
- Commit work regularly and ensure a detailed README.md is present.

## Requirements
### Part 1: Access the New York Times API
- Correctly construct `query_url`.
- Create and populate `reviews_list`.
- Loop through pages and handle API rate limits.
- Preview results and convert to DataFrame.
- Extract titles and convert "keywords" to strings.
- Generate titles list for The Movie Database queries.

### Part 2: Access The Movie Database API
- Prepare and execute search queries.
- Loop through titles and handle exceptions.
- Retrieve and process movie details.
- Append results to `tmdb_movies_list`.
- Preview results and convert to DataFrame `tmdb_df`.

### Part 3: Merge and Clean the Data for Export
- Merge DataFrames on title.
- Clean list columns and remove characters.
- Drop duplicates and reset index.
- Export to CSV without index.

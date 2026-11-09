# Letterboxd Stars Analysis

## Project Overview & Objectives

This project analyzes movie ratings and user preferences on Letterboxd to explore audience behavior, genre popularity, and rating patterns across different movie release years.

**Key Objectives:**
- Identify the most popular and highest-rated movie genres.
- Examine overall movie rating distributions and user rating behavior.
- Compare ratings of older and newer movies.
- Investigate the relationship between movie release years and ratings.
- Explore whether movie popularity is associated with higher ratings.

## Dataset

**Source:** [Letterboxd Movie Ratings Data – Kaggle](https://www.kaggle.com/datasets/samlearner/letterboxd-movie-ratings-data)

The dataset consists of three CSV files containing movie information, user profiles, and movie ratings.

| File | Records | Description |
|---|---:|---|
| `movie_data.csv` | 285,963 | Movie details, genres, release years, and metadata |
| `ratings_export.csv` | 11,078,167 | Movie ratings submitted by users |
| `users_export.csv` | 8,139 | User profiles and activity information |

*These figures represent raw record counts before data cleaning and validation.*

**Sampling Note:**

The dataset was collected from approximately 4,000 of the most active Letterboxd users in a given month, rather than a random sample of the platform's user base. As a result, the findings may not represent the preferences and rating behavior of all Letterboxd users.



## Tools & Technologies

- **Python (Pandas):** Data exploration, cleaning, and statistical analysis.
- **Jupyter Notebook:** Interactive analysis and documentation.
- **SQL:** Data querying and relational analysis (planned).
- **Power BI:** Interactive dashboard development (planned).
- **Git & GitHub:** Version control and project documentation.

## Data Exploration & Quality Assessment

The initial exploration assessed data completeness, consistency, duplicates, and relationships across the three datasets.

### Data Quality Summary

| Check | Key Findings |
|---|---|
| CSV Structure | 573 malformed parsed records identified in the Movies dataset. |
| Missing Values | 3.73% of movie records have missing genres, while 2.65% have missing release years. |
| Duplicates | No duplicates detected in structurally valid movie records, user records, or valid rating identifiers and user-movie pairs. |
| Rating Validation | All 11,078,167 ratings fall within the expected range of 1–10. |
| Release Years | 23 records contain years requiring further review. |
| Relational Integrity | 99.98% of ratings match both a movie and a user. |
| Genre Coverage | 22.05% of structurally valid movie records have missing or empty genres. |

### Key Observations

- The Movies CSV contains malformed multiline descriptions, requiring structural repair before further processing.
- Missing genre and release year information may affect specific analyses.
- Most rating records have valid references, although unmatched movie and user IDs require investigation.
- The dataset shows no duplicate records within the validated subsets examined.

**Note:** Movie-related findings are preliminary and will be reassessed after repairing the malformed CSV structure. No original data was modified during exploration

## Data Cleaning & Preparation

## Exploratory Data Analysis (EDA)

## SQL Analysis

## Statistical Analysis

## Power BI Dashboard

## Key Findings & Insights

## Limitations

## Project Structure

## References


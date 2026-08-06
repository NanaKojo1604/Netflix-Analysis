# Netflix Catalog Analysis

Exploratory data analysis of Netflix's movie and TV show catalog, using the
[Netflix Movies and TV Shows dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)
from Kaggle (8,807 titles).

## Project Overview
This project explores Netflix's content library to uncover patterns in
content type, geographic distribution, catalog growth over time, and genre
composition. Built as part of a data analyst portfolio project.

## Tools Used
- Python (pandas, matplotlib, seaborn)
- Jupyter Notebook
- Git & GitHub

## Process
1. Loaded and inspected the raw dataset (structure, data types, missing values)
2. Cleaned missing data — filled `director`, `cast`, and `country` with
   "Not Specified"; dropped rows with missing `date_added`, `rating`, or
   `duration` (under 0.15% of rows affected)
3. Performed exploratory analysis and visualized key patterns
4. Documented findings as business insights

## Key Insights
- **Movies dominate the catalog** — ~70% of titles (6,131 of 8,807) are
  movies, with the remaining ~30% TV shows.
- **The US leads content volume** — 2,818 titles, more than triple the next
  closest country.
- **TV-MA is the most common rating** — ~36% of titles, suggesting the
  catalog skews toward mature audiences.
- **Catalog growth peaked in 2019** — additions grew sharply from 2016–2019,
  then declined in 2020–2021, plausibly tied to COVID-19 production
  disruptions.
- **International Movies is the top genre** — followed by Dramas and
  Comedies, reflecting a diverse catalog with a strong international focus.

## Files
- `analysis.ipynb` — full analysis notebook (cleaning, EDA, visualizations, insights)
- `NetflixData_Kaggle/netflix_titles.csv` — raw dataset

## Next Steps
Potential extensions: correlate genre with rating, deeper time-series
analysis by content type, or compare international vs. domestic content
growth.

- **TV-MA and TV-14 lead ratings for both Movies and TV Shows** — though
  Movies span a wider ratings range (R, PG-13, PG, G), while TV Shows
  cluster more tightly around mature/teen ratings.
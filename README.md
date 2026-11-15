# Zuber — SQL & Data Analysis

**Author:** Ana Paula Takezawa  
**Education:** MBA in Data Science and Artificial Intelligence — TripleTen Brasil

## Project Overview

This project focuses on analyzing Chicago's taxi market for Zuber, a new ride-hailing company preparing to launch its operations in the city.

The objective is to explore taxi market data, identify leading taxi companies and popular destinations, and investigate the relationship between weather conditions and trip duration.

The analysis combines SQL queries and Python-based exploratory data analysis to extract insights from operational and weather datasets.

## Business Objectives

- Analyze the number of trips completed by taxi companies.
- Compare the performance of selected taxi companies.
- Identify the most popular drop-off neighborhoods in Chicago.
- Investigate the relationship between weather conditions and trip duration on Saturdays for trips from the Loop to O'Hare International Airport.

## Tools & Technologies

- **SQL** — Data extraction, filtering, aggregation, JOIN operations, and conditional logic.
- **Python** — Data analysis and processing.
- **Pandas** — Data manipulation and exploratory data analysis.
- **Matplotlib** — Data visualization.
- **Requests & BeautifulSoup** — HTML data extraction.

## Project Workflow

### 1. Data Understanding

Reviewed the database schema and explored four tables:

- `neighborhoods` — Chicago neighborhood information.
- `cabs` — Taxi and taxi company information.
- `trips` — Trip details, including timestamps, duration, and locations.
- `weather_records` — Hourly weather observations.

### 2. SQL Analysis

Developed SQL queries to:

- Calculate the number of trips per taxi company on November 15–16, 2017.
- Compare Yellow and Blue taxi companies from November 1–7, 2017.
- Compare Flash Cab and Taxi Affiliation Services with all other companies.
- Identify the Loop and O'Hare neighborhoods.
- Classify hourly weather conditions as `Good` or `Bad`.
- Retrieve Saturday trips from the Loop to O'Hare and associate them with corresponding weather conditions.

### 3. Exploratory Data Analysis (Python)

Used Pandas and Matplotlib to analyze two datasets:

- Taxi companies and their number of trips.
- Average trips by drop-off neighborhood in November 2017.

The analysis included data inspection, data type verification, identification of the top 10 destination neighborhoods, and visual comparisons.

### 4. Weather Impact Analysis

Analyzed 200 Saturday trips from the Loop to O'Hare, comparing average trip duration under two weather classifications:

- `Bad` — Rain or storm conditions.
- `Good` — Other weather conditions.

Calculated average trip duration and created a comparative visualization.

## Key Findings

### Taxi Market Analysis

Flash Cab recorded the highest number of trips, with **19,558 trips** on November 15–16, 2017, followed by Taxi Affiliation Services with 11,422 trips.

In the November 1–7 comparison, the combined category of other taxi companies accounted for the largest number of trips, followed by Flash Cab and Taxi Affiliation Services.

### Popular Destinations

The Loop and River North were the leading drop-off neighborhoods in November 2017, with average daily trip counts of approximately:

- **Loop:** 10,727 trips.
- **River North:** 9,524 trips.
- **Streeterville:** 6,665 trips.

### Weather and Trip Duration

The analysis showed a difference in average trip duration between the two weather classifications:

| Weather Conditions | Trips | Average Duration |
|---|---:|---:|
| Bad | 26 | 41.00 minutes |
| Good | 174 | 31.66 minutes |

Trips under adverse weather conditions took approximately **9.34 minutes longer on average**, representing an increase of about 29.5% compared with trips under other weather conditions.

These results indicate an association between adverse weather conditions and longer trip durations. However, the analysis does not establish a causal relationship.

## Conclusion

This project demonstrates how SQL and Python can be combined to explore transportation data, identify market patterns, and investigate operational factors that may influence trip duration.

The findings highlight the leading taxi companies, the most frequent destination neighborhoods, and differences in trip duration under varying weather conditions.

The analysis provides an initial understanding of Chicago's taxi market and illustrates the value of data-driven approaches to business analysis.

## Data Sources

The datasets were provided as part of the Data Science and Artificial Intelligence MBA program at TripleTen Brasil.

Weather data was extracted from the following HTML source:

[Chicago Weather Records — November 2017](https://practicum-content.s3.us-west-1.amazonaws.com/data-analyst-eng/moved_chicago_weather_2017.html)

The original SQL database and CSV datasets are not included in this repository.

## Repository Structure

```text
zuber-sql-data-analysis/
│
├── README.md
├── notebooks/
│   └── zuber_sql_analysis.ipynb
├── images/
└── .gitignore
```

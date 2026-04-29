# Explore US Bike Share Data

A data analysis project using **R** to explore bike share usage patterns across three major U.S. cities: Chicago, New York City, and Washington, D.C.

This project was completed as part of the [Udacity Programming for Data Science with R Nanodegree](https://www.udacity.com/course/programming-for-data-science-nanodegree--nd118).

---

## Project Overview

Using data provided by [Motivate](https://www.motivateco.com/), a leading U.S. bike share system operator, this analysis investigates ridership patterns from the first six months of 2017 (January through June). The goal is to answer three data-driven questions about how, when, and by whom the bike share systems are used.

---

## The Three Questions

### Question 1: When do riders use the system most?
Explores the most popular month, day of week, and hour of day across all three cities. The hourly and monthly trend charts reveal clear commuter-driven peaks in New York City and Chicago, and a flatter leisure-oriented distribution in Washington.

### Question 2: How long are trips, and does that differ by user type?
Compares mean and median trip duration (in minutes) between Subscribers (annual/monthly members) and Customers (short-term pass holders) in each city. Customers consistently take longer rides, consistent with leisure use, while Subscribers take shorter routine commutes.

### Question 3: Who are the riders?
Examines user type composition across all three cities, with gender breakdown and birth year statistics for New York City and Chicago (where that data is available). Subscribers dominate all three cities, male riders outnumber female riders in both NYC and Chicago, and the typical rider was born in the mid-1980s to early 1990s.

---

## Visualizations

| # | Chart | Type |
|---|-------|------|
| 1 | Trips by Hour of Day | Line chart |
| 2 | Trips by Month | Grouped bar chart |
| 3 | Mean Trip Duration by City and User Type | Grouped bar chart |
| 4 | User Type Distribution by City | Stacked bar chart |
| 5 | Gender Distribution: NYC and Chicago | Grouped bar chart |

---

## Key Findings

- New York City and Chicago show clear morning (8 AM) and evening (5-6 PM) commuter peaks; Washington does not.
- All three cities see growing ridership from January through June, consistent with seasonal weather effects.
- Customers ride approximately 2-3 times longer on average than Subscribers in every city.
- Subscribers make up the large majority of trips in all three cities.
- Male riders account for roughly 70-75% of riders in NYC and Chicago.
- The most common rider birth year is in the mid-1980s, placing the core user base in their late 20s to mid-30s in 2017.

---

## Dataset

Randomly selected data for the first six months of 2017. All three files share six core columns:

| Column | Description |
|--------|-------------|
| Start Time | Timestamp when the trip began |
| End Time | Timestamp when the trip ended |
| Trip Duration | Duration in seconds |
| Start Station | Name of the starting dock station |
| End Station | Name of the ending dock station |
| User Type | Subscriber or Customer |

Chicago and New York City also include:

| Column | Description |
|--------|-------------|
| Gender | Rider gender (Male / Female) |
| Birth Year | Rider birth year |

---

## Files

```
Explore_bikeshare_data.ipynb   # Main analysis notebook (R kernel)
chicago.csv                    # Chicago bike share data
new_york_city.csv              # New York City bike share data
washington.csv                 # Washington D.C. bike share data
README.md                      # This file
```

---

## How to Run

1. Clone this repository.
2. Open `Explore_bikeshare_data.ipynb` in Jupyter Notebook with an R kernel (IRkernel).
3. Ensure the following R packages are installed: `ggplot2`, `dplyr`, `lubridate`.
4. Run all cells in order from top to bottom.

To install the required packages in R:
```r
install.packages(c("ggplot2", "dplyr", "lubridate"))
```

---

## Tools and Libraries

- **R** programming language
- **ggplot2** for data visualization
- **dplyr** for data manipulation and summarisation
- **lubridate** for date/time parsing
- **Jupyter Notebook** with IRkernel (R kernel)

---

## About

This project is part of **Operation Graduate**, a structured plan to complete a Bachelor of Science in Data Analytics at Western Governors University by August 2026.

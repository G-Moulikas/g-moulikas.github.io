# Cyclistic Bike-Share Analysis

## Overview

This repository contains the analysis performed for the Cyclistic bike-share case study. The goal of this analysis was to understand how casual riders and annual members use Cyclistic bikes differently, with the aim of developing marketing strategies to convert casual riders into annual members.

## Data

The data used in this analysis consists of historical bike trip data from Cyclistic, specifically from Q1 2019 and Q1 2020. The datasets are:

-   `Divvy_Trips_2019_Q1.csv`
-   `Divvy_Trips_2020_Q1.csv`

## Analysis

The analysis was performed using R, with the following key steps:

1.  **Data Collection:** The datasets were loaded into R using the `read_csv` function from the `readr` package.
2.  **Data Cleaning and Preparation:**
    * The datasets were combined into a single dataframe.
    * Columns were renamed for consistency.
    * Calculated ride length.
    * Removed rows with errors.
    * Added columns for day, month, year, and day of the week.
3.  **Descriptive Analysis:**
    * Calculated summary statistics for ride length and other variables.
    * Aggregated data by rider type (member/casual) and day of the week.
4.  **Visualization:**
    * Created visualizations to compare the number of rides and average ride duration between member and casual riders.
    * Visualizations were created to show the number of rides, and average ride duration per weekday, and per rider type.
5.  **Export Summary File:**
    * Created a csv file that contains the average ride length per day of the week, and per rider type.

## Key Findings

* There is a significantly higher number of rides from members compared to casual riders across all days of the week.
* Casual riders have a significantly longer average ride duration compared to members across all days.
* Member ride durations are relatively consistent and shorter, suggesting they use the service for quick commutes or errands.
* Casual riders usage increases during the weekends, and they ride for longer periods of time during the weekends.

## Suggestions

Based on the analysis, the following suggestions were made:

* Targeted membership tiers (Explorer, Commuter)
* Highlighting the value of longer rides.
* Incentivizing off-peak longer rides.
* Further investigation into the "why" behind longer rides.

## Files

* `Cyclistic-Case-Study.Rmd`: The R Markdown file containing the analysis code.
* `Cyclistic-Case-Study.docx`: A knit of the R Markdown file.
* `avg_ride_length.csv`: A CSV file containing the average ride length by rider type and day of the week.

## How to Reproduce

To reproduce this analysis, you will need:

* R and RStudio installed.
* The following R packages: `tidyverse`, `lubridate`, and `ggplot2`.
* The datasets `Divvy_Trips_2019_Q1.csv` and `Divvy_Trips_2020_Q1.csv`.

1.  Clone this repository.
2.  Open `Cyclistic-Case-Study.Rmd` in RStudio.
3.  Run the code chunks in the R Markdown file.
4.  The output will be generated in the RStudio viewer and the `avg_ride_length.csv` file will be created.

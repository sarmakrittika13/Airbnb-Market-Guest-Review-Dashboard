# Airbnb Market & Guest Review Dashboard

**Created by Krittika Sarma**

An interactive Power BI dashboard exploring Airbnb listing distribution, room types, asking prices, and guest review activity across 10 cities.

## Dashboard Preview

![Airbnb Market & Guest Review Dashboard](Dashboard/Airbnb%20Dashboard.png)

## Project Overview

This project uses Airbnb listing and review data to explore differences across cities and room types. The dashboard presents key counts and rating averages, compares listing volumes across cities, examines room-type mix, and shows review activity over time. A City slicer allows users to filter the report and explore asking prices by room type within a selected city.

## Business Questions and Findings

### 1. Which cities have the most Airbnb listings?

Paris has the largest listing count in the dashboard, followed by New York and Sydney. Hong Kong has the fewest listings among the cities shown.

### 2. How does the room-type mix vary across cities?

Entire-place listings form the largest share in most of the cities shown. Private rooms are also a substantial part of the mix, while hotel and shared rooms account for smaller portions overall.

### 3. How does asking price vary by room type?

The dashboard compares average asking price across room types for the city selected in the slicer. Use the City slicer to explore a specific market. Prices are in local currencies, so the chart should be interpreted within one city at a time.

### 4. How has review activity changed over time?

Review volume increased substantially through the years shown, reached a peak around 2019, and then declined. The latest year may be incomplete, so the final drop should not be interpreted as a full-year decline without checking the date coverage.

### 5. What are the overall listing and host counts represented in the data?

The dashboard shows approximately **280K listings**, **182K hosts**, and **5M reviews**. These are rounded KPI-card values.

## Dashboard Features

- **KPI cards:** Host count, listing count, average asking price, average listing rating, and review count.
- **Listings by city:** Compares listing volume across the 10 cities.
- **Listings by city and room type:** Shows how room-type composition differs by market.
- **Average asking price by room type:** Compares room types in the city selected in the City slicer.
- **Reviews by year:** Shows review activity over time.
- **City slicer:** Filters the report to selected cities.

## Dataset

The project uses the **Airbnb Listings & Reviews** dataset from Maven Analytics:

[Open the Airbnb Listings & Reviews dataset](https://mavenanalytics.io/data-playground/airbnb-listings-reviews)

The source files contain approximately **279,712 listing records** and **5,373,143 review records** across **10 cities**. Listing fields include host, location, property, room type, price, and rating information. Review records include listing IDs, review IDs, reviewer IDs, and review dates.

## Tools

- Microsoft Power BI Desktop
- Power Query for data import and preparation
- DAX measures for dashboard metrics

## Interpretation Notes

- Listing prices are recorded in each city’s local currency. Prices should not be compared across cities without currency conversion.
- The dataset does not include bookings, occupied nights, or realized revenue. Asking price is not revenue, and this dashboard does not measure occupancy.
- Review volume counts recorded reviews; it is not a direct count of bookings or, by itself, a measure of guest satisfaction.
- Some listing rating and host-response fields are blank. Missing values should not be interpreted as zero.
- The latest year in the review trend may be incomplete, so its total should be interpreted cautiously.
- Findings above are descriptive observations from the dashboard, not causal conclusions.

## Repository Contents

- `Dashboard/` — dashboard screenshot
- `README.md` — project overview, business questions, findings, data source, and interpretation notes

The Power BI report file and raw data files are not included in this repository. Use the dataset source link above to access the data.

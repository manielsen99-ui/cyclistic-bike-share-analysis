# Processed Data

## Overview
The processed dataset was created by cleaning, validating, and transforming raw bike-share trip data to ensure accuracy and consistency for analysis.

## Cleaning Steps Applied
- Removed records with missing start or end timestamps
- Removed rides with zero or negative durations
- Standardized rider type values to `member` and `casual`
- Converted timestamps to datetime format
- Created derived fields for analysis

## Derived Fields
- ride_length_minutes
- day_of_week
- hour_of_day
- month (YYYY-MM)

## Aggregated Outputs
Processed data was summarized into analysis-ready tables, including:
- Total rides by rider type
- Average ride length by rider type
- Ride counts by day of week
- Ride counts by hour of day
- Monthly ride trends
- Monthly average ride lengths

These aggregated tables are stored in the `/tables` folder.

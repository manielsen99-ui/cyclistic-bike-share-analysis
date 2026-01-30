# Cleaning Log (June 2022 – May 2023)

## Source files
Processed 12 monthly CSV files from the Divvy/Cyclistic public dataset (June 2022 through May 2023).

## Row counts
- Total rows read: 5,829,030
- Rows kept for analysis: 5,828,463

## Cleaning rules applied
1. **Required timestamps**: dropped rows where `started_at` or `ended_at` is missing or unparseable.
2. **Valid rider type**: kept only `member_casual` values of `member` or `casual`.
3. **Positive duration**: dropped rows where `ended_at` ≤ `started_at` (non‑positive ride length).

## Rows removed by rule
- Missing/unparseable timestamps: 0
- Invalid rider type: 0
- Non‑positive duration: 567

## Derived fields created (from `started_at`)
- `ride_length_minutes`
- `day_of_week`
- `hour_of_day`
- `month` (YYYY‑MM)

Note: Raw data files were not modified; all cleaning occurred via scripted transformations.

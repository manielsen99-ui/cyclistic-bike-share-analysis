# Assumptions & Limitations

## Assumptions
- The public Divvy/Cyclistic trip dataset accurately reflects recorded rides for the period analyzed.
- `member_casual` correctly identifies rider membership status.
- Ride start time (`started_at`) is an appropriate anchor for day/hour/month usage patterns.

## Limitations
- **No user-level tracking**: Riders are not uniquely identifiable across trips, so this analysis focuses on trip behavior, not individuals.
- **Station data may be missing** for some rides (e.g., dockless or system changes). This project does not impute station fields.
- **Time zones**: Datetimes were parsed consistently during processing. If the source contains mixed time zones, that could affect fine-grained time patterns.
- **Outliers**: Very long rides can inflate average ride length. Median ride length is reported using a sample-based approximation.

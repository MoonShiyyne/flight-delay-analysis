
# Flight Delay Analysis — BTS On-Time Performance, October 2025

Coursework for an AI/ML course at FSU, analyzing US domestic departure delay patterns.

## Source

Bureau of Transportation Statistics, Reporting Carrier On-Time Performance (1987–present).
Downloaded from https://www.transtats.bts.gov/ as the prezipped October 2025 file:
605,844 flights, 110 fields, all US domestic flights operated by reporting carriers.

## Files

**`clt_oct2025.csv`** — 13,713 rows. Charlotte Douglas (CLT) departures operated by
American Airlines (AA) and PSA Airlines (OH), which together account for ~84% of CLT
departures. All 110 original fields retained, plus derived columns for scheduled
departure hour, day of week, schedule padding, and delay absorbed in flight.

**`top10_hubs_oct2025.csv`** — Departures from the ten busiest US origin airports,
reduced to 24 fields relevant to delay timing and causes.

## Notes

The five delay-cause fields (CarrierDelay, WeatherDelay, NASDelay, SecurityDelay,
LateAircraftDelay) are only populated when a flight arrives 15 or more minutes late,
so any percentages derived from them describe significant delay rather than total delay.

Negative delay values indicate early departures or arrivals and are retained, not clipped.

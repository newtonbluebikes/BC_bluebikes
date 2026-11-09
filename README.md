# BC_bluebikes
Boston College Bluebikes Use Data Jan 2025 through October 2026

# Newton Bluebikes Trips

Interactive map and trip data for Bluebikes bikeshare trips that start or end at a station in Newton, MA.

**Live map:** see the GitHub Pages link in this repository's About section.

## Files

| File | What it is |
|---|---|
| `index.html` | Interactive map of trips to and from the Boston College T station. Opens in any web browser. |
| `newton-bluebikes-trips-2025-01_to_2026-10.csv` | Every Bluebikes trip that started or ended at one of Newton's 16 stations, January 2025 – October 2026 (44,189 trips). |

## Data sources

- **Trips:** Bluebikes system data, monthly trip history files, January 2025 – October 2026.
- **Stations:** Bluebikes station list (updated August 21, 2026), plus Upper Falls Greenway Pettee Square (station K13452), which opened August 26, 2026.
- **Basemap:** MassGIS town boundaries, open space and major hydrography; MassDOT roads; MassGIS MBTA rapid transit lines.

## Notes on the trip file

- Newton stations are identified by station ID: the 15 stations with IDs beginning `N3`, plus `K13452` (Upper Falls Greenway Pettee Square).
- Station `N32008` appears as "Langley Lot" in March–April 2025 and as "Union St at Herrick Rd" afterward; both are included.
- Added columns: `duration_min` (trip length in minutes), `month`, `trip_type` (within Newton, from Newton, to Newton), `start_in_newton`, `end_in_newton`.
- Bluebikes removes staff trips and trips under 60 seconds before publishing. 33 trips in this file last more than 24 hours and are likely bikes that weren't docked properly.
- The data does not identify riders, so trips by students or other groups can't be separated out.

## Notes on the map

- Lines connect the Boston College T station to the station at the other end of each trip. Line thickness shows total trips, on the same scale for every filter.
- Filters: months (all, school year, summer), direction (both, leaving BC, arriving at BC) and bikes (all bikes or e-bikes only).
- The side panel includes summary statistics on e-bike use and an About this data section with sources and caveats.
- Round trips (started and ended at Boston College T) are shown as a dashed ring around the station.
- School year = September–May; summer = June–August.
- Distances are straight-line miles from the Boston College T station.

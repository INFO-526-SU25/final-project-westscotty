# Data

-   **Vesuvius**: This dataset explores seismic events detected at the famous Mount Vesuvius in Italy. It comes from the [Italian Istituto Nazionale di Geofisica e Vulcanologia (INGV)](https://www.ingv.it/)'s [Data Portal](https://data.ingv.it/en/). The raw data was saved as individual CSV files from the GOSSIP website and some values were translated from Italian to English.
-   **Sourced**: [Vesuvius CSV Data](https://raw.githubusercontent.com/rfordatascience/tidytuesday/main/data/2025/2025-05-13/vesuvius.csv)

# Codebook for Vesuvius Dataset

## Variable Names and Descriptions:

| variable | description |
|:--------------------------|:--------------------------------------------|
| event_id | Unique identifier for each seismic event recorded. |
| time | Date and time when the seismic event occurred, in UTC format. |
| latitude | Geographic latitude of the seismic event location in decimal degrees. |
| longitude | Geographic longitude of the seismic event location in decimal degrees. |
| depth_km | Depth of the seismic event epicenter in kilometers below the surface. |
| duration_magnitude_md | Duration magnitude (Md) of the seismic event, a measure of its energy release. Md is often used for smaller magnitude events, and negative values can indicate very small events (microearthquakes). |
| md_error | Estimated error margin ("plus or minus") for the duration magnitude measurement. |
| area | Geographic area where the seismic event was recorded. In this case, the Mt. Vesuvius area. |
| type | Classification of the seismic event, such as "earthquake" or "eruption." |
| review_level | Level of review the data has undergone. The data might be raw (preliminary) or revised (reviewed by someone). |
| year | Calendar year when the seismic event occurred. |

## Data Types:

| variable              | class     |
|:----------------------|:----------|
| event_id              | integer   |
| time                  | datetime  |
| latitude              | double    |
| longitude             | double    |
| depth_km              | double    |
| duration_magnitude_md | double    |
| md_error              | double    |
| area                  | character |
| type                  | character |
| review_level          | character |
| year                  | integer   |
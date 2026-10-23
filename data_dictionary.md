# Data Dictionary

This file explains the column structures used in the CSV files of this dataset. This database is designed as a set of linked tables to analyze ice avalanche dynamics.

## glaciers.csv (Metadata)
* **glacier_id**: Unique identifier for the glacier (Format: CountryCode-3Letters).
* **name**: Common name of the glacier.
* **canton**: Swiss canton where the glacier is located.
* **latitude**: WGS84 decimal latitude.
* **longitude**: WGS84 decimal longitude.
* **elevation_min_m**: Minimum elevation in meters above sea level.
* **elevation_max_m**: Maximum elevation in meters above sea level.
* **years_covered**: Years covered in data.

## events.csv (Ice Avalanche Database)
* **event_id**: Unique identifier for the avalanche event.
* **date_start**: Start date of the event in ISO 8601 format (YYYY-MM-DD).
* **date_end**: End date of the event in ISO 8601 format (YY-MM-DD). 
* **time_start**: Start time of the event (HH:MM) if captured by monitoring cameras.
* **time_end**: End time of the event (HH:MM) if captured by monitoring cameras. 
* **magnitude_vol_m3**: Estimated volume of the ice avalanche in cubic meters.
* **geometry_notes**: Observations on glacier geometry at the release area prior to the event.
* **ice_flow_velocity_m_day**: Recorded ice flow velocity from monitoring systems around the time of the event.
* **weather_condition**: Link or description of weather/climate conditions (e.g., temperature spike, precipitation).
* **trigger_type**: Suspected mechanism controlling the release.
* **image_reference**: Filename of the repeat imagery from monitoring cameras capturing the event.
* **data_source**: Origin of the cataloged event (e.g., monitoring cameras, Geoformer preliminary catalog, published literature).

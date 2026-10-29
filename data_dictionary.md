# Data Dictionary

This file explains the column structures used in the CSV files of this dataset. This database is designed as a set of linked tables to analyze ice avalanche dynamics.

## glaciers.csv (Metadata)
* **glacier_id**: Unique identifier for the glacier (Format: CountryCode-3Letters).
* **name**: Common name of the glacier.
* **canton**: Swiss canton where the glacier is located.
* **latitude**: WGS84 decimal latitude.
* **longitude**: WGS84 decimal longitude.
* **elevation_min**: Minimum elevation in meters above sea level.
* **elevation_max**: Maximum elevation in meters above sea level.
* **years_covered**: Years covered in data.
* **corr_weather_stat**: Corresponding weather station. 
## events.csv (Ice Avalanche Database)
* **event_id**: Unique identifier for the avalanche event (**glacier_id**_**date_start**_index).
* **date_min**: Start date of the event in ISO 8601 format (YYYY-MM-DD).
* **date_max**: End date of the event in ISO 8601 format (YY-MM-DD). 
* **time_min**: Start time of the event (HH:MM) if captured by monitoring cameras.
* **time_max**: End time of the event (HH:MM) if captured by monitoring cameras. 
* **magnitude_area**: Estimated area of the ice avalanche in pixels.
* **magnitude_vol**: Estimated volume of the ice avalanche in m3.
* **category_magnitude**: Category of the magnitude of the avalanche in relation to alpine avalanches (small < 50'000 m3; medium < 300'000; large > 300'000).
* **geometry_notes**: Observations on glacier geometry at the release area prior to the event (wedge / slab).
* **ice_flow_velocity_m_day**: Recorded ice flow velocity from monitoring systems around the time of the event.
* **av_temperature**: Average temperature between start and end of event.
* **sum_precipitation**: Sum of precipitation over XXX days.
* **sum_sunshine**: Sum of sunshine hours over XXX days.  
* **trigger_type**: Suspected mechanism controlling the release.
* **image_reference**: Filename of the repeat imagery from monitoring cameras capturing the event.
* **data_source**: Origin of the cataloged event (e.g., monitoring cameras, Geoformer preliminary catalog, published literature).
* **notes**: observational comments - common observations may get a new column.

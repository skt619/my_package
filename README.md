Coastal Vulnerability (Census Blocks)
=====================================
2010 Census **blocks** in the coastal study area. Each record has a block-level
**Vulnerability Index** `vi_mean` in [0,1] (higher = more vulnerable).

`coastal_vulnerability.geojson`
----------------------------------------
A **GeoJSON export** of the same features/attributes as the shapefile; a single-file
alternative for web/non‑ESRI tools (e.g., Leaflet/Mapbox/QGIS/GeoPandas).

`coastal_vulnerability.zip`
-----------------------------------------------
The zip file contains a standard **ESRI Shapefile**. After unzipping,
keep the files together. These are usable in **ArcGIS**, **QGIS**, and **GeoPandas**.

Required shapefile parts:
- `coastal_vulnerability.shp`  (geometry)
- `coastal_vulnerability.shx`  (index)
- `coastal_vulnerability.dbf`  (attributes)
  
Recommended:
- `coastal_vulnerability.prj`  (coordinate system)
  
Optional:
- `coastal_vulnerability.cpg`  (text encoding)
  
(Any extra sidecar like `.prj` and `.cpg` are not required to read the data.)

Columns (attributes)
--------------------
- `STATEFP10`  — 2‑digit 2010 state FIPS
- `COUNTYFP10` — 3‑digit 2010 county FIPS
- `TRACTCE10`  — 6‑digit 2010 tract code
- `BLOCKCE10`  — 4‑digit 2010 block code
- `GEOID10`    — 15‑digit unique block ID (concat of the above)
- `state_name` — state name
- `county_name`— county name
- `tract_name` — tract label
- `block_name` — block label
- `INTPTLAT10` — internal point latitude (deg)
- `INTPTLON10` — internal point longitude (deg)
- `vi_mean`    — vulnerability index [0,1]

`coastal_vulnerability.csv`:
-----------------------------------------------
Contains only attributes (no geometry). 

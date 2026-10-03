# Northern-Territory-Mining-Spatial-Data-Visualisation

## Overview
This project explores Northern Territory Government open spatial data relating to mineral titles. The data was processed and visualised using QGIS to demonstrate the use of spatial data, GIS tools, attribute queries, and map visualisation techniques.

The project focuses on transforming raw open spatial data (shp files) into clear and meaningful visual outputs, including mineral title maps, title information, associated party information, and dynamic map highlighting.

## Data Source
The project uses mineral title data from the **Northern Territory Government Open Data Portal**(https://data.nt.gov.au/dataset/strike---northern-territory-mineral-titles).

The main datasets used are:
- `MIN_TITLE_PROD_GRNT`
- `MIN_TITLE_PROD_APPL`

The datasets contain spatial and attribute information relating to mineral titles, including:
- Title ID
- Title type
- Status
- Grant date
- Expiry date
- Party / holder information
- Interest percentage
- Holder type
- Spatial geometry

## Tools and Technologies
- **QGIS** – Spatial data processing and visualisation
- **QGIS Virtual Layers** – Creating customised attribute views
- **OpenStreetMap** – Basemap and geographic context
- **GeoPackage** – Spatial data storage
- **QGIS Print Layout** – Map and information presentation
- **QGIS Atlas** – Dynamic map generation
- **Rule-based Symbology** – Dynamic feature highlighting

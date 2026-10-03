# Northern Territory Mining Spatial Data Visualisation

## Overview

This project explores **Northern Territory Government open spatial data** relating to mineral titles. The data was processed and visualised using QGIS to demonstrate the use of spatial data, GIS tools, attribute queries, and map visualisation techniques.

The project focuses on transforming raw open spatial data (SHP files) into clear and meaningful visual outputs, including mineral title maps, title information, associated party information, and dynamic map highlighting.


## Data Source

The project uses mineral title data from the **Northern Territory Government Open Data Portal**:

[Strike - Northern Territory Mineral Titles](https://data.nt.gov.au/dataset/strike---northern-territory-mineral-titles)

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
- **QGIS Virtual Layers** – Creating customised attribute views using SQL
- **OpenStreetMap** – Basemap and geographic context
- **NT Geology Province 2.5M** – Geological geographic context
- **GeoPackage** – Spatial data storage
- **QGIS Print Layout** – Map and information presentation
- **QGIS Atlas** – Dynamic map generation
- **Rule-based Symbology** – Dynamic feature highlighting


## Visualisation of Results

### QGIS Project Workspace

QGIS built-in **OpenStreetMap** data and **NT Geology Province 2.5M** were added as background layers to provide geographic and geological context for the mineral title boundaries.

This provides additional geographic context and makes the mineral title spatial data easier to interpret.

![QGIS Project Workspace](https://github.com/kkkkabi/Northern-Territory-Mining-Spatial-Data-Visualisation/blob/main/Image/1.%20NT%20Mineral%20Titles%20Project%20Workspace.png)


### QGIS Print Layout

A QGIS **Print Layout** was created to combine the spatial map with the corresponding title and party information.

The aim was to present spatial and attribute information in a concise and readable format.

The layout contains:

- Mineral title map
- OpenStreetMap basemap
- Geological context
- Selected title highlight
- Title information
- Party information

![QGIS Print Layout](https://github.com/kkkkabi/Northern-Territory-Mining-Spatial-Data-Visualisation/blob/main/Image/3.%20Printed%20Layer%20with%20Title%20Information.png)


### Virtual Layers

Two QGIS **Virtual Layers** were created to display key title information and party information for each individual mineral title.

The Virtual Layers use SQL to select and organise relevant attributes from the mineral title dataset.

The **Title Information** Virtual Layer includes:

- Title ID
- Title type
- Status
- Title status
- Granted date
- Expiry date

The **Party Information** Virtual Layer includes:

- Party name
- Interest percentage
- Holder type

The Virtual Layers are linked to the QGIS Atlas so that the information displayed corresponds to the currently selected mineral title.


### Dynamic Map Visualisation Using QGIS Atlas

QGIS **Atlas** functionality was used to create dynamic map pages for individual mineral titles.

The current mineral title can be selected using the Atlas feature list. When the selected title changes, the map and associated information are updated accordingly.

The dynamic output includes:

- Mineral title location
- Selected title highlight
- Title information
- Party information

![Dynamic Title Information](https://github.com/kkkkabi/Northern-Territory-Mining-Spatial-Data-Visualisation/blob/main/Image/2.%20Virtual%20Layer%20with%20Title%20Information%20(Dynamic).png)


## Workflow

The overall workflow can be summarised as:

```text
NT Government Open Data
        ↓
Import SHP Data into QGIS
        ↓
Add OpenStreetMap / Geological Context
        ↓
Save Spatial Data as GeoPackage
        ↓
Create Virtual Layer – Title Information
        ↓
Create Virtual Layer – Party Information
        ↓
Create QGIS Print Layout
        ↓
Create QGIS Atlas
        ↓
Apply Rule-based Symbology
        ↓
Dynamic Title Highlighting
        ↓
Dynamic Title & Party Information
        ↓
Export Map to Image
```

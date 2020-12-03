
## WEB GIS WITH OPEN SAUCE

Hi there,

Welcome to my blog series on WebGIS using open source tools and technologies with the Free and Open Source Software for Geospatial Applications(FOSS4G) Stack. This 7 somewhat long-section series aims to introduce you to the beauty of WebGIS and some of the cool things you can pull off with it especially with absolutely free tech stacks. It'll run the gamut from basic to advanced operations using several tools, technologies, and frameworks. A WebGIS project would be implemented towards the end of the series to apply the knowledge gained. All resources used in this series could be found [in this GitHub](https://github.com/jeafreezy/WebGIS-with-Opensausce-Stack) repository. You would also find a playlist for this series on my Youtube channel sometime in the future, kindly [subscribe](https://www.youtube.com/channel/UCdYaK054HlTq49qOJDTh2oA) and turn on post notification to be informed when it's released. I do hope you have a lovely read and find this series helpful.

_Disclaimer: This series does not aim to reinvent the wheel and thus would include links to several existing resources that explain a particular concept well, also, in no way does the open-source emphasis in this series makes me a hater of proprietary software. I wrote this based on the little experience I have acquired using these tools and with the sole goal of contributing to the knowledge space. My ultimate focus is on what gets the job done and not the tools battle._
## Table of Contents:

### [Section 1: Quick Introduction to GIS and WebGIS.]()

- What is GIS?
- What is WebGIS?  
- Why FOSS4G?

### [Section 2: Overview of the tools, technologies, and frameworks for WebGIS.]()

- Spatial Database
  - PostgreSQL/POSTGIS
- Software client
  - QGIS
- Command line utilities
  - GDAL/OGR(ogr2ogr,ogrinfo etc)
  - shp2pgsql
  - psql
- Middleware
  - Geoserver
  - Apache tomcat server
  - ngrok
- Frontend Javascript libraries and frameworks.
  - Leaflet 
  - Mapbox GL
  - turfjs
  - Openlayers
  - **React JS**


### [Section 3: Methodology workflow chart for a WebGIS and *Enterprise GIS*]()

### [Section 4: QGIS and the spatial Database(PostGIS) ]()

- Installation of QGIS, PostgreSQL, and PostGIS
- Introduction to PostGIS
- Working with vector layers in PostGIS
- Working with raster layers in PostGIS => psql,raster2pgsql.
- Connecting PostGIS with QGIS
- Layer upload/download between PostGIS and QGIS.

### [Section 5: A dive into Geoserver](./section5.md)
- Overview and Installation of Geoserver  
- Creating a workspace
- Creating a Store
- Connecting Geoserver with PostGIS
    -Adding layers from PostGIS
- Loading and previewing layers in Geoserver
- Creating a layer group
- Styling a layer in Geoserver
    - Save and apply .sld styles from QGIS to layers in Geoserver
- OGC services and Geoserver
- Connecting Geoserver with QGIS
- Installing additional plugins in Geoserver
### [Section 6: A dive into Openlayers]()
- Pre-requisites
- Creating a basic map view
- Adding base maps
- Connecting OpenLayers to Geoserver

    - Load layers through WFS requests
    - Load layers through WMS requests
- Using plugins with Openlayers
### [Section 7: A dive into Leaflet JS]()
- Pre-requisites
- Creating a basic map view
- Adding base maps
- Connecting Leaflet JS to Geoserver

    - Load layers through WFS requests
    - Load layers through WMS requests
- Using plugins with Leaflet JS
### [Section 8: A dive into Mapbox GL]()
- Pre-requisites
- Creating a basic map view
- Adding base maps
- Connecting Mapbox GL to Geoserver

    - Load layers through WFS requests
    - Load layers through WMS requests
- Using plugins with Mapbox GL
### [Section 9: The beauty of the Command-Line Utilities(GDAL/OGR)](./section9.md)
- Installation of GDAL/OGR
- Working on data with *ogrinfo*
- GIS data formats conversion with  *ogr2ogr*

### [Section 10: A simple WebGIS App project ]()
- Pre-requisites
- Getting the data
- File conversion with *ogr2ogr*
- Styling on QGIS
- Loading on PostGIS
- Loading on Geoserver
- Choosing a frontend library
- Basic web template
- Making requests to Geoserver
- Additional styling
- Steps on hosting our web app

### [Section 11: Bonus]()
- Bonus
  - Python and GIS
  - Django overview

### REFERENCES




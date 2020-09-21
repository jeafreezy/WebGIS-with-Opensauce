# WEB GIS WITH OPENSAUCE STACK

Welcome to my blog series on WebGIS using open source tools and technologies and the Free and Open Source Software for Geospatial Applications(FOSS4G) Stack. This 7 section series aims to introduce you to WebGIS and some of the cool things you can pull off with it. It'll run the gamot from basic to some advanced operations using several WebGIS tools,technologies and frameworks. A WebGIS project would be implemented towards the end of the series to apply the knowledge gained. All resources used in this series could be found [in this GitHub](https://github.com/jeafreezy/WebGIS-with-Opensausce-Stack) repository. I do hope you have a lovely read and find this series helpful.

## Table of Contents:

### [Section 1: Introduction to GIS and WebGIS.](./section1.md)

- What is GIS ?  
- What is WebGIS ?  
- Why FOSS4G ?

### [Section 2: Overview of the tools,technolgies and frameworks for WebGIS.](./section2.md)

- Spatial Database
  - PostgreSQL/POSTGIS
- Software clients
  - QGIS
- Command line utilities
  - GDAL/OGR(ogr2ogr,ogrinfo etc)
  - shp2pgsql
  - psql
- Middleware
  - Geoserver
  - Apache tomcat server
- Frontend Javascript libraries and framework.
  - Leaflet 
  - Mapbox GL
  - turfjs
  - Openlayers
  - **React JS**

### [Section 3: Methodology workflow chart for a WebGIS and *Enterprise GIS*](./section3.md)

### [Section 4: QGIS and the spatial Database(PostGIS) ](./section4.md)

- Installation of QGIS, PostgreSQL and PostGIS
- Introduction to PostGIS
- Working with vector layers in PostGIS
- Working with raster layers in PostGIS => psql,raster2pgsql.
- Connecting PostGIS with QGIS
- Layer upload/download between postGIS and QGIS.

### [Section 5: A dive into Geoserver](./section5.md)
- Overview and Installation of Geoserver  
- Creating a workspace
- Creating a Store
- Connecting Geoserver with PostGIS
    -Adding layers from postGIS
- Loading and previewing layers in Geoserver
- Creating a layer group
- Styling a layer in Geoserver

    - Save and apply .sld styles from QGIS to layers in Geoserver
- OGC services and Geoserver
- Connecting Geoserver with QGIS
- Installing additional plugins in Geoserver
### [Section 6: A dive into Openlayers](./section6.md)
- Pre-requisites
- Creating a basic mapview
- Adding basemaps
- Connecting openlayers to Geoserver

    - Load layers through WFS requests
    - Load layers through WMS requests
- Using plugins with Openlayers
### [Section 7: A dive into Leaflet JS](./section7.md)
- Pre-requisites
- Creating a basic mapview
- Adding basemaps
- Connecting Leaflet JS to Geoserver

    - Load layers through WFS requests
    - Load layers through WMS requests
- Using plugins with Leaflet JS
### [Section 8: A dive into Mapbox GL](./section8.md)
- Pre-requisites
- Creating a basic mapview
- Adding basemaps
- Connecting Mapbox GL to Geoserver

    - Load layers through WFS requests
    - Load layers through WMS requests
- Using plugins with Mapbox GL
### [Section 9: The beauty of the Command Line Utilities(GDAL/OGR)](./section9.md)
- Installation of GDAL/OGR
- Working on data with *ogrinfo*
- GIS data formats conversion with  *ogr2ogr*

### [Section 10: A simple project: Coronovirus distribution WebAPP ](./section10.md)
- Pre-requisites
- Getting the data
- File conversion with *ogr2ogr*
- Styling on QGIS
- Loading on postGIS
- Loading on Geoserver
- Choosing a frontend library
- Basic web template
- Making requests to Geoserver
- Additional styling
- Steps on hosting our web app

### REFERENCES

- Spatial Database
- Software clients
- Command line utilities
- Middleware
- Frontend Javascript libraries and framework.



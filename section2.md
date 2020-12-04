# Overview of the Tools, Technologies, and Frameworks For WebGIS.

In the previous [section](https://jeafreezy.hashnode.dev/section-1-quick-introduction-to-gis-and-webgis-cki8iqqgh02a6hps15dgm5463), we had a quick introduction to GIS and WebGIS.We explained what a GIS is and dived a little into some core of WebGIS. This section aims to go further by introducing you to some of the open-source tools used in WebGIS. There are a lot of them, but we would only discuss the ones we would use in the rest of the series. We'll look at them categorically;

- Spatial Database
  - [PostGIS](https://postgis.net/): It's is the spatial extension to PostgreSQL object-relational database. It adds supports for the storage of spatial data and allows spatial operation and queries to be run in SQL. The software was initially released on April 19, 2001. We would look into how we can use this database to store and query spatial data in future sections.
  
  
  
- Software clients
  - [QGIS](https://qgis.org/) : This is a desktop GIS client. It allows users to create, edit, visualize, analyze, and publish geospatial information and it runs major flavors of operating systems and Android devices. The software, written in C++, Python, and Qt was initially released in July 2002.
  
- Command-line utilities
  - [GDAL/OGR)](https://gdal.org/): The Geospatial Data Abstraction Library(GDAL) and the OpenGIS Simple Features Reference Implementation(OGR) are powerful libraries for reading and writing raster and vector geospatial data formats. The software written in C, C++, and python, was released on the 8th of June,2000. The original author was Frank Warmerdam but it's currently maintained by developers at the Open Source Geospatial Foundation. It supports a lot of raster and vector formats and this has made it widely used for spatial data conversion even in various software like QGIS, ArcGIS,gvSIG, Grass GIS, Google Earth, etc.

  - shp2pgsql: This is a tool developed for easy conversion of ESRI shapefiles into SQL suitable for insertion into the PostGIS/PostgreSQL database.
  
- Middleware
  - [Geoserver](http://geoserver.org/): This is a server written in Java that allows users to share, process, and edit geospatial data. It publishes data from any major data sources using open standards. It can be easily connected to web-based frontend libraries such as leaflet, Mapbox, OpenLayers, etc. using Open Geospatial Consortium(OGC) compliant services.
  
  - [Apache tomcat server](http://tomcat.apache.org/): Released in 1999 and written in Java. It's a platform-independent tool and a popular Java-based HTTP server that provides functionalities of interacting with java servlets.
  
  - [ngrok](https://ngrok.com/): This service enables the creation of public URLs accessible over the internet. For example, the Geoserver can be installed on an Apache Server on our local machine, we can then use ngrok to listen to the server at a particular port and it'll generate a URL that can be used to access the GeoServer over the internet. This is a fast way to test run developments, before hosting the Geoserver on the cloud or any web hosting platform.
  
- Frontend Javascript libraries and framework.
  - [Leaflet](https://leafletjs.com/): It is a simple, lightweight javascript library for developing interactive maps on the web. It was initially released on May 13, 2011. It is mobile-friendly, has a well-documented API, and a lot of plugins. 
   
  - [Mapbox GL](https://docs.mapbox.com/mapbox-gl-js/example/): According to the official documentation, It is a JavaScript library for interactive, customizable vector maps on the web. It takes map styles that conform to the Mapbox Style Specification, applies them to vector tiles that conform to the Mapbox Vector Tile Specification, and renders them using WebGL.
  
  - [Openlayers](https://openlayers.org/): It is a javascript library that makes it easy to put a dynamic map on any web page. It can display map tiles, vector data, and markers loaded from any source. OpenLayers was initially released on June 26, 2006. It can be connected to Geoserver via OGC compliant services.
 


That would be all for this section, we would pick these tools one at a time and explore more of their functionalities in subsequent sections. I hope you've been able to learn one or two things. Kindly share if you feel this would be beneficial to someone out there.


# Section 4: QGIS And The Spatial Database(PostGIS)
## Introduction

Q**GIS** & Post**GIS**,both have something in common. Can you take a quick guess? Yeah,you probably guessed right. It's the **GIS** in their names. Does this suggest that they are both a GIS software? Well maybe or maybe not. What I do know is that often times,these duo are enough for most of your analysis needs.
Welcome to another secion of this series,in the [previous](https://jeafreezy.hashnode.dev/section-3-webgis-architecture-ckizi2fny01t6pys1glkk41im) section we looked into WebGIS architecture, in this section we would look into QGIS and PostGIS,how to install them on our computer and connect them together. At the end of this section would be some helpful resources to help you learn more about them and dive deeper.


TL;DR

C'mon it's not too long,so read it up! Quick expo: You can use the table of contents below to skip to any section of choice :)


## Contents

- What is PostGIS?
- Why Use PostGIS?
- PostgreSQL/PostGIS Installation
- QGIS Installation
- Connecting QGIS to PostGIS
- Uploading Shapefiles to PostGIS with the Shapefile Loader
- Uploading raster to PostGIS with raster2pgsql & psql
- Resources


## What is PostGIS?

Before diving into PostGIS, I would like us to quickly scratch the surface of databases world. Databases are systems for storing,retrieving and sometimes performing analysis on structured data. It has three major components;

1. **Functions:** These are operations we can perform on the data stored in a database.
2. **Data Types:** These are the kinds and format of data that can be stored in a database.
3. **Indexes:** These are the faster actions and ways to retrieve data from the database.

_Let's relate the whole system described above to our local banks. We use our banks to store and retrieve our money(database).There are some acceptable currencies we store in the bank E.g USD,EUR,NGN etc(Data Types),also there are some activities we can perform on our money. E.g transfer,exchange,deposit,invest etc(Functions) and finally there are faster ways we can retrieve our money E.g Point of Sales(POS),Automated Teller Machines(ATMs),Online Banking etc(Indexes)._


There are two types of databases--relational(stores data in tabular format i.e rows and columns) and non-relational(stores data in a document based format i.e non-tabular,often called No SQL) and the common laguage used for communicating with the database is the SQL(Structured Query Language).


Just like databases we have three major components for PostGIS:

1. **Spatial Data Types:** This refer to shapes such as point, line, and polygon;

2. **Spatial Indexes and Bounding Box:** It is used for efficient processing of spatial operations.

3. **Spatial Functions:**They are used for querying of spatial properties and relationships.

The combination of spatial data types, indexes, and functions provide a flexible structure for optimized performance and analysis.

PostGIS is an extension to a popular,powerful and free open-source relational database management system called PostgreSQL. It  turns the PostgreSQL Database Management System into a spatial database by adding support for the three features described above: spatial types, indexes, and functions. The open-source nature of PostGIS gives it the flexibility to use several other open source software like Geoserver,QGIS etc. PostGIS store and manipulate spatial objects like any other object in the database.


### Why Use PostGIS?

* Free

* Paul Ramsey,the co-founder of PostGIS calls it a GIS without a GIS :)

* It's easy to install( CREATE EXTENSION POSTGIS;)

* It's can be used for enterprise applications

* PostGIS can connect with several clients e.g QGIS,Geoserver

* and lots more...


## PostgreSQL/PostGIS installation

This video demonstrates the installation of PostgreSQL 13.1,PGAdmin 4 and PostGIS 3.1 on a  windows 10 (64bit) machine using the software installation file downloaded from the official website. As a dark mode fan, I went ahead to customize my PGAdmin 4 to support dark mode(who don't like dark mode anyway?). If you have them installed already you can skip this or watch,you might probably learn a new thing.:)

### Video
%[https://www.youtube.com/watch?v=nmqDkzmxKDU&list=PLz9AoTLQKsZgoiT9UHCDb70KmujjNnhWV&index=2]

### Useful Links

- [PostGIS website](https://postgis.net)

## QGIS Installation

This video demonstrates the installation of QGIS 3.16 on a windows 10 (64bit) machine using the software installation file downloaded from the official QGIS website.The installation is very straightforward,thanks to QGIS contributors for the well documented website so If you want to install on another operating system,I bet you won't face any issues if you follow the documentation keenly. That was what I did :). If you have QGIS installed already you can skip to the next section.

### Video
%[https://www.youtube.com/watch?v=8qhqihxpUVI&t=20s]

### Useful Links

 - [QGIS website](https://qgis.org)

## Uploading Shapefiles to PostGIS with the shapefile loader

PostGIS is not so useful if we stop at the installation and since it's a spatial extension to PostgreSQL I demostrated  in this video the uploading of a vector layer(shapefile) to PostGIS using the Shapefile loader that came installed with it and I also did the visualization within PostGIS. Do you know you can visualize data in PostGIS? Well, Check the video to see that.

### Pre-requisites

- PostGIS installation(See above)

### Video

%[https://www.youtube.com/watch?v=KXZGO8S4siA&t=28s&pbjreload=101]

### Useful Links

[EPSG](https://epsg.io)

## Connecting QGIS to PostGIS

This video demonstrates how to connect to PostGIS using the browser panel in QGIS.

### Pre-requisites

- PostGIS installation(See above)
- QGIS installation( See above)

### Video

%[https://www.youtube.com/watch?v=lWDHjQZ7q_g&t=3s]

### Useful Links

[Link](https://www.youtube.com/watch?v=eddcoyLtqqs)

## Uploading raster to PostGIS with raster2pgsql & psql

This video demonstrates how to upload a raster data into PostGIS using the raster2pgsql from our command line.

### Pre-requisites

- PostGIS installation(See above)
- QGIS installation( See above)

### Video

%[https://www.youtube.com/watch?v=vAQk9kG3YH4]
 

## Conclusion

In this section we looked into PostGIS and QGIS. We installed them on our computer and went ahead to upload data into PostGIS from within QGIS and the command line. I hope you found it helpful. In the next section we would look into Geoserver, another powerful open source software. That would be all for now,see you next section!

## Resources

* Curious on where I got the word GIS without a GIS? Check out this presentaion from Paul Ramsey,PostGIS Co-Founder. at the STL [PostGIS Day,2019](https://www.youtube.com/watch?v=g4DgAVCmiDE&t=2260s)

* Playlist to dive deeper into [Spatial SQl and Postgis](https://www.youtube.com/watch?v=fgS1eVPPBiElist=PLAxJ4-o7ZoPcvp0ETujkLVCmKIGj-YvlG) by the great Dr. Quiseng wu!

* This [interactive](https://learn.crunchydata.com/training/postgis) learning platform by Crunchy Data is super great to get up and running with learning PostGIS. 

* Official Introduction to [PostGIS](https://postgis.net/workshops/postgis-intro/introduction.html)

# Quick Introduction to GIS and WebGIS

Welcome to the first section of this series on *WebGIS with Opensauce*. This section aims to give you a taste of the beauty of Geographic Information Systems(GIS) and Web GIS. At the end of this section, hopefully you would have an understanding of these terms and be able to explain in simpler and easy-to-digest terms to your friends and coworkers. Diving in  🏄🏻;


### **What is GIS ?**  

Several existing explanations,quotes,definitions and terms have attempted to capture the description of a GIS in a few sentences,while some of them are absolutely valid and succint it might be a bit technical to assimilate by a layman. If you ask me what a GIS is,I'll gladly respond with this beautiful and simple explanation below;

>GIS,an acronym for Geographic Information System, is a transformational technology that exists to make our life easier and the world a better place,if rightly harnessed.
>

More technically, a geographic information system (GIS) is a computer based system used for collecting,storing,manipulating and analyzing spatial data i.e data that can be referenced to a particular location on earth. This suggests that GIS is data driven!

There is a lot more to GIS,you could check out this blog post by [GIS lounge](https://www.gislounge.com/what-is-gis/) to learn about the history,job prospects,uses,applications and lots more. 

### **What is WebGIS ?**

The World Wide Web(WWW) has transformed everything and GIS is no exception. WebGIS is an advanced form of Geographic Information Systems available on web platforms. It kicked off as a GIS running in web browsers and has evolved into Web GIS serving desktop and mobile clients. It is any GIS that uses Web technology to communicate between some components: a GIS server(identified by a URL) and a client (a web browser,a desktop application, or a mobile application). The communication is via Hypertext Transfer Protocol(HTTP/HTTPS) and the format of the response can be an HTML, binary image, XML(Extensible Markup Language),GML(Geography Markup Language) or JSON(JavaScript Object Notation). The overaching goal of this technology is to allow user to dynamically access,share and manipulate geospatial data on the web no matter the platform or protocol.

### **A brief look at the GIS Server and OGC Web Services**

The GIS Server is a software that actively listens for specific requests sent by a client. These requests could be for different OGC compliant services e.g a GetMap request in Web Map Service(WMS), GetFeature request incase of Web Feature Service(WFS),getCoverage requests in Web Coverage Services (WCS) etc. The GIS server loads the dataset been requested (e.g. a shapefile or a raster) renders it, splits the image into tiles and sends to the requesting client. Every time a client interacts with the map, the GIS server receives requests and sends image tiles as response at a very fast speed. There are various open source options to choose for a GIS Server,a number of them are listed in this blog post by [GIS Lounge](https://www.gislounge.com/open-source-gis-applications) , but for this series we would be using [GeoServer](http://geoserver.org/). 

Geoserver is one of the most commonly used GIS server. It has a web based administration interface and deploys datasets in OGC compliant protocols, which makes it an ideal option.

OGC services are specified by the Open Geospatial Consortium(OGC) that allows all kinds of geospatial functionality. They allow the exchange of geographic data across the web. Extensible Markup Language(XML)-based Geographic Markup Language(GML) is used for exchange of information.Some examples;

- Web Map Services(WMS): It is an OGC standard that allows users to remotely access georeferenced map images via hypertext transfer protocol (HTTPS) requests.
  
- Web Feature Service(WFS): It is an interface specified by the Open GIS Consortium (OGC) that allows for the exchange of geographic data across the Web. Users are able to create,delete,update or lock a feature instance.
    
- Web Coverage Service(WCS): It offers multi-dimensional coverage data for access over the Internet. e.g raster imageries. Check [here](https://www.ogc.org/docs/is) for other OGC services.

### **The WebGIS clients**

Clients of a web GIS can include local desktop applications, and native mobile apps or any browser-support applications.Several open source and proprietary application programming interfaces (APIs) are used for creating web and mobile frontend applications that consumes OGC compliant web services. These include [Open Layers](https://openlayers.org), [Leaflet](https://leafletjs.com),[Mapbox GL](https://mapbox.com), [ArcGIS APIs](https://developers.arcgis.com/javascript/ ) etc. In order to provide an intuitive user experience, these client apps and APIs often abstract the details of all the web service requests that occurs in background.

#### **Characteristics and key elements of a Web GIS**

A webGIS must satisfy the following;

1. Global reach by HTTP/HTTPS i.e the server must have a specific Uniform resource locator(URL) on the web so that client can access it easily.
2. Support a large number of users simultanuously: requires high performance and scalability.
3. Better cross-platform capability: -Different Web browsers: IE, Firefox, G. Chrome for diverse OSs (Win, Linux, Mac OS, iOS). etc.

#### **Applications of Web GIS**

The WebGIS has diverse applications. Some of them are listed below;

1. Collaborative collection of Geospatial Data e.g Geoportals,clearing houses,SDI etc.
2. Volunteering Geographic Information System e.g [Openstreetmaps](https://openstreetmap.org)
3. WebGIS can be used to design and plan governments projects like urban flood management ,natural disasters etc.


### **Challenges of WebGIS**

- Accessibility for the disabled
- Security
- Data quality
- System performance
- Assessibility in poorly connected locations
- Maintenance costs etc.
  
### **Why Open Source Software ?**

Web GIS can be implemented in diverse ways. But this series is focusing on Free and Open SOurce Software for Geospatial Applications because of the following reasons;

1. **FREE**
2. Acessibility i.e easy to follow,so you won't need to make any purchase before you follow this series through.
3. A large community support.
4. Control: We have a total control of the software hence we can customize it to our need and desire. etc.


I hope the above contents have introduced you to webGIS, next up is **[section 2](./section2.md)**, where we'll look at the at the tools,technologies and frameworks we'll use for the rest of this series.



### **References:**

[What is WebGIS,How does it work and what are its applications?](https://www.vizexperts.com/webgis)

[WebGIS Explained-5 Essential Elements and What is WebGIS?](https://www.geo-jobe.com/videos/web-gis-explained-5-essential-elements-web-gis/)  

[What is WebGIS?](https://www.igi-global.com/dictionary/online-urban-information-systems/32458)    

[What is the differnce between WebGIS and Internet GIS?](https://www.gislounge.com/difference-web-gis-internet-gis/)
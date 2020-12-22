# WebGIS Architecture

In previous sections, we introduced GIS, WebGIS, and some tools and libraries used for WebGIS. We explained a GIS and dived a little into some core of WebGIS, we went further to categorically introduce some of the open-source tools that are used in WebGIS projects. A picture is worth a thousand words, they say. In that light, my goal in this section is to explain the architectural workflow of a WebGIS without being verbose. It is expedient we understand that there is no de facto WebGIS architecture, workflows are dependent on their application context, however, they all rely on a three-tier client/server architecture.

TL;DR

In summary, implementing a WebGIS relies on the client/server model. The whole operation is broken down into client facing side and the server-side. The client can be a web browser or a desktop GIS software and the server-side consists of a Web Server(e.g Apache Tomcat), Web GIS server(e.g Geoserver), and a Database(e.g PostGIS). Below is a graphic that explains the whole process.

![DJANGO WALK THROUGH.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1608612004594/i1qjucXO4.png)

Figure 1: WebGIS architecture

### What is a Client/Server Architecture?

Leaving all the technicality aside, let me try to explain it to you using an example I think we could all relate to. Let's look at it in this direction, a customer(client) visits a restaurant to make some orders, the waiter(server) is always listening to customer orders or requests, they'll process it, communicate with the chefs(database ) to prepare the client's request/order and return a response to the client. This is tantamount to how WebGIS works and even the web generally. We have a database that stores our spatial data e.g PostGIS, it's installed on or connected to a server such as Apache tomcat for example that's installed on a Linux machine and always listens to requests, on the server is also a Web GIS server such as a Geoserver instance installed to handle OGC services requests such as WFS and WMS, these requests are processed and sent back to the browsers via the frontend libraries such as Leaflet, OpenLayers that makes the requests and displays it beautifully in the browser. 
<iframe src="https://giphy.com/embed/fVWPYi4EoLATm" width="auto" height="326" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/hateplow-google-paris-hateplow-fVWPYi4EoLATm">via GIPHY</a></p>

All these happen in a jiffy, and depends on a lot of factors, for example, your internet connectivity and of course, there are a lot of processes that occur in the background, but since the goal is to make us understand the whole process with minimal words I won't scare us away with super complex technical details.

Still don't get it yet?

<iframe src="https://giphy.com/embed/26tP4gFBQewkLnMv6" width="auto" height="365" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/warnerarchive-hanna-barbera-flintstones-a-flintstone-christmas-26tP4gFBQewkLnMv6">via GIPHY</a></p>

Okay, I get you, let's look at it again. Let's assume you want to order a pizza. The first thing you'll probably do is to pick up your mobile phone or your computer, open your browser(the client) and type in the URL(https://dominos.com). Do you know what you just did is make a request to the server where https://dominos.com website files are stored? Lol, just so you know, the word "Server" is actually a system too, that's probably in a faraway location from us and we could use our system as a server too (we would do this in future sections). The server would return the response in HTML, CSS, and Javascript files to the client(your browser) since that's the only language your browser understands, it'll consume them and display them to us in nice layouts that we see on the website, then we proceed to make the order.

<iframe src="https://giphy.com/embed/mCRJDo24UvJMA" width="auto" height="348" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/dog-shiba-inu-typing-mCRJDo24UvJMA">via GIPHY</a></p>

Additionally, while navigating the websites, they're a lot of requests and response operations that undergoes in the background. For example, when we make an order, the order details and information are sent to the server to get the order processed and packaged for delivery. (This is a typical POST request). That process is similar to what happens in WebGIS. A user pans around the map, the browser or the GIS software sends a request to the server, the server process it, and returns a response back to the client to display. Sometimes if a request is frequent the response is cached to reduce latency and for a better user experience. 

<iframe src="https://giphy.com/embed/39jJqoSw7tFa4etjDM" width="auto" height="270" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/yevbel-39jJqoSw7tFa4etjDM">via GIPHY</a></p>

Phew! that's a lot, I know. Thanks so much for sticking around! I do hope it's comprehensive enough. I promised not to be verbose so I'll drop my pens here. Please do not forget to share if you find this article helpful. 

Finally, future sections are more of coding, software, and library installation. I would be demonstrating these activities on my youtube channel. Kindly [subscribe](https://www.youtube.com/channel/UCdYaK054HlTq49qOJDTh2oA) if you haven't. Thanks! And see you in the next section! 





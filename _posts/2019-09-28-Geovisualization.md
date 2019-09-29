---
layout: post
title: Geovisualization
---

Consider building a pizza from scratch. Every pizza starts with a base of crust. Added to this are a variety of layers including tomato sauce, cheese, and any number of meat and vegetable toppings. Of the range of available options, a pizza can be customized to match the tastes of each customer. In the same way that a pizza is the final product of a combination of many layers, geovisualization starts with a base map and combines many forms of geographical and social data. 

<img src="https://st3.depositphotos.com/1177973/12516/i/950/depositphotos_125166678-stock-photo-layers-of-pizza-isolated-on.jpg" width="200" height="200"/>

<p style="font-size:75%;"> <i>Source: Stock image from https://depositphotos.com/125166678/stock-photo-layers-of-pizza-isolated-on.html  </i></p>


As put by Markus Jobst, Jürgen Döllner, and Olaf Lubanski in the book entitled <i>"Communicating Geoinformation Effectively With Virtual 3d City Models"</i>: geovisualization or geographical visualization may be defined as <i><b>"a set of tools and techniques supporting geospatial communication and information analysis through the use of interactive maps." </b></i>$^1$ Geovisualization is a particularly useful way of putting data into context by showing how the measures of a particular variable compare relative to their neighbours and compared to other areas of interest on the map. 


<img src="https://www.vizionz.nl/images/serv-gis/gisdata.jpg" width="200" height="300"/>

<p style="font-size:75%;"> <i>Source: "Geographic Information Systems." Visionz. https://www.vizionz.nl/services/geographic-information-systems </i></p>

<b>Example 1: Transit maps for route planning</b>

When faced with the question of what bus you can take to get from point A to point B, reviewing a stack of bus schedules is an option. While it is certainly possible, this may take an excessive amount of time to go through. Luckily, more digestible alternatives exist! For example, the network of local bus routes may be presented on a map of the Greater Vancouver Area. This quickly shows an observer which neighbourhoods are serviced by buses and where the closest bus lines may be found. Taken a bit further, tools such as Google Maps allow users to input starting and destination details. This allows the sofware to provide a map of options the users can take to where they need to go. These maps are customizable and can show satellite images on top on base layer if the user so desires. 

<b> Geovisualization in Python </b>

Now that we've touched on what is a geovisualization is, it is possible for us begin making our very own using Python. The libraries ```geopandas``` , ```fiona``` and ```matplotlib``` provide all the necessary tools get started. ```geopandas``` allows ```pandas``` to work with geographic data files while relying on ```fiona``` for file access and ```matplotlib``` for plotting. Example 2 belows shows how a simple geovisualization may be constructed.


<b>Example 2: GeoPandas in action</b>

Using these three libraries we can plot our base layer using the code below:

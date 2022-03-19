# Mapping_Earthquakes


## Overview

The purpose of this project is to visualize the magnitudes of earthquakes all over the world for the last week.

Earthquake GeoJSON from the [USGS](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php)  website is used to retrieve the geographical coordinates and magnitudes of earthquakes for the last seven days.  Fault lines GeoJSON is retreived from the following github repository: https://github.com/fraxen/tectonicplates.

JavaScript, and the D3.js library is used to traverse the data retrieved from the [USGS](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php) site and [githup repository](https://github.com/fraxen/tectonicplates), and then the open source JavaScript Library, Leaflet.js is used to plot the data on three different Mapbox API maps.

## Results

The page is loaded with a default view of the earth in street mode. All earthquakes for the past seven days are represented; the larger the radius and darker the color, the larger the earthquake.  Fault lines are also displayed by default. The lower right corner contains a legend explaining the color to magnitude correlation.

![Default View](/Earthquake_Challenge/Resources/Default.png)

Clicking on a  marker opens up a popup with the magnitude and location details. 

![Popup](/Earthquake_Challenge/Resources/Popup.png)

A control in the upper right hand corner allows users to switch between map views.

![Map](/Earthquake_Challenge/Resources/satellite.png)

The same control also allows users to apply layers. In the following example, only tectonic plates are chosen:

![Filter](/Earthquake_Challenge/Resources/FilteredOverlay.png)



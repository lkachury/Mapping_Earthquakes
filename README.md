# Mapping_Earthquakes

## Overview 
An earthquake map was previously created with two different maps and the earthquake overlay. The purpose of this analysis is to now see the earthquake data in relation to the tectonic plates’ location on the earth, see all the earthquakes with a magnitude greater than 4.5 on the map, and see the data on a third map.

## Resources
### Data Source 
- 

### Software
- Visual Studio Code 1.69
- JavaScript and HTML
- Bootstrap 3 and CSS
- Chrome Developer Tools
- D3 (Data Driven Document) Javascript library

## Results
For Reference: 
- The complete [index.html]() file used to build the webpage
- The complete [charts.js]() file used to build the graphs in the webpage
- The complete [style.css]() file used to style the webpage

### Deliverable 1: Add Tectonic Plate Data
Using JavaScript, Leaflet.js, and geoJSON data, tectonic plate data was added using ```d3.json()```, added the data using the ```geoJSON()``` layer, set the tectonic plate ```LineString``` data to stand out on the map, and added the tectonic plate data to the overlay object with the earthquake data.

1. The tectonic plate data is added as a second layer group:
<br /> ![image](https://user-images.githubusercontent.com/108038989/193414721-e6d5b86c-ef8d-49b8-a4e0-af682b48f39a.png)

2. The tectonic plate data is added to the overlay object: 
<br /> ![image](https://user-images.githubusercontent.com/108038989/193414746-182f986b-6b5a-402d-b5ac-21bebe10d8c7.png)

3. The ```d3.json()``` callback is working and does the following: 
    - The tectonic plate data is passed to the ```geoJSON()``` layer
    - The ```geoJSON()``` layer adds color and width to the tectonic plate lines
    - The tectonic layer group variable is added to the map
    <br /> ![image](https://user-images.githubusercontent.com/108038989/193414800-5be13f8f-114e-49ec-b127-9f546eb9e1dc.png)

4. The earthquake data and tectonic plate data displayed on the map when the page loads:
<br /> ![image](https://user-images.githubusercontent.com/108038989/193414686-4371dab8-b6f2-460c-a6c0-399646c2ff79.png)

### Deliverable 2: Add Major Earthquake Data
Using JavaScript, Leaflet.js, and geoJSON data, major earthquake data was added to the map using ```d3.json()```. Color was added and the radius of the circle markers were set based on the magnitude of earthquake, and a popup marker for each earthquake was added that displays the magnitude and location of the earthquake using the GeoJSON layer, ```geoJSON()```.

1. The major earthquake data is added as a third layer group:
2. The major earthquake data is added to the overlay object:
3. The ```d3.json()``` callback is working and does the following:
   - Sets the color and diameter of each earthquake.
   - The major earthquake data is passed to the ```geoJSON()``` layer. 
   - The geoJSON() layer creates a circle for each major earthquake, and adds a popup for each circle to display the magnitude and location of the earthquake.
   - The major earthquake layer group variable is added to the map.
4. All the earthquake data and tectonic plate data are displayed on the map when the page loads and the datasets can be toggled on or off:

### Deliverable 3: Add an Additional Map 
Using JavaScript and Leaflet.js, a third map style was added to the earthquake map.

1. A third map tile layer is created:
2. The third map is added to the overlay object:
3. All the earthquake data and tectonic plate data are displayed on the all maps of the webpage:

## Summary

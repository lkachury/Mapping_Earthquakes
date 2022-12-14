# Mapping_Earthquakes

## Overview 
An earthquake map was previously created with two different maps and the earthquake overlay. The purpose of this analysis is to now add a third map and two more earthquake overlays: earthquake data in relation to the tectonic plates’ location on the earth and all the earthquakes with a magnitude greater than 4.5 on the map.

## Resources
### Data Source 
- Earthquakes [GeoJSON](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson) 
- Earthquakes >4.5 mag [GeoJSON](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/4.5_week.geojson)
- Tectonic Plate [GeoJSON](https://raw.githubusercontent.com/fraxen/tectonicplates/master/GeoJSON/PB2002_boundaries.json)

### Software
- Visual Studio Code 1.69
- JavaScript and HTML
- Bootstrap 3 and CSS
- Chrome Developer Tools
- D3 (Data Driven Document) Javascript library

## Results
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
<br /> ![image](https://user-images.githubusercontent.com/108038989/193417012-0a21e9b1-869e-4a92-95da-b347a7437ac9.png)

2. The major earthquake data is added to the overlay object:
<br /> ![image](https://user-images.githubusercontent.com/108038989/193417024-827ef516-7d26-4906-bbbd-74ca2e9f9df4.png)

3. The ```d3.json()``` callback is working and does the following:
   - Sets the color and diameter of each earthquake: <br /> ![image](https://user-images.githubusercontent.com/108038989/193417181-befc872d-9a04-40a5-bb35-25134bf30e88.png)  
   - The major earthquake data is passed to the ```geoJSON()``` layer 
   - The geoJSON() layer creates a circle for each major earthquake, and adds a popup for each circle to display the magnitude and location of the earthquake.
   - The major earthquake layer group variable is added to the map: <br /> ![image](https://user-images.githubusercontent.com/108038989/193417224-dcaafd28-043d-4c26-b5fc-599b1bcc9b2a.png)

4. All the earthquake data and tectonic plate data are displayed on the map when the page loads and the datasets can be toggled on or off:
    - With All Data On: <br /> ![image](https://user-images.githubusercontent.com/108038989/193416753-6a8d9abe-576c-4ec9-82cc-1e3fb07e2dc3.png)
    - With Major Earthquakes Off: <br /> ![image](https://user-images.githubusercontent.com/108038989/193416821-a021699f-a010-4b02-b509-d287ad6dd587.png)
    - With Tectonic Plates Off: <br /> ![image](https://user-images.githubusercontent.com/108038989/193416862-2079d08d-bea2-41ca-af73-df362e2405d6.png)
    - With Earthquakes Off: <br /> ![image](https://user-images.githubusercontent.com/108038989/193416902-4768c935-427f-4e9b-ae3c-b6ca0d6e6c83.png)

### Deliverable 3: Add an Additional Map 
Using JavaScript and Leaflet.js, a third map style was added to the earthquake map.

1. A third map tile layer is created: <br /> ![image](https://user-images.githubusercontent.com/108038989/193417672-1682c3ef-a60d-4d08-9ad3-29d11c75ba2c.png)
2. The third map is added to the overlay object: <br /> ![image](https://user-images.githubusercontent.com/108038989/193417699-8890fc20-128d-4fff-a362-20633f10f3c8.png)
3. All the earthquake data and tectonic plate data are displayed on the all maps of the webpage: <br /> ![image](https://user-images.githubusercontent.com/108038989/193417638-6cd2cba1-1867-4587-af17-e8b0082cd817.png)

## Summary
An earthquake map was created with three different maps (Streets, Satellite, Dark) and three different earthquake overlays (Earthquakes, Tectonic Plates, and Major Earthquakes). 

# Mapping_Earthquakes
![image](https://user-images.githubusercontent.com/112978144/222587473-aad984b7-a9a9-4367-b8d1-1476e653160c.png)


# Visualize Earthquake Data
In order to visualize earthquake data for module challenge we use Leaflet API to create a geographical map with GeoJSON earthquake data that originates from a website.

# Overview of the Project
 An informative, eaily accessable and interactive map is created to display GeoJSON earthquake data in relation to tectonic plate's location on earth for "Disaster Reporting Network", a nonprofit company that provides data driven storytelling on disasters around the world.
# Deliverable 1
In step 1, second layer group variable for the tectonic plate data is added.

In Step 2, a reference to the tectonic plate data to the overlay object is added.

In Step 3, using d3.json() callback method, a call is made to the tectonic plate data using the GeoJSON/PB2002_boundaries.json data from this GitHub repositoryLinks to an external site.

Inside the d3.json() method following steps have been taken

Passed the tectonic plate data to the geoJSON() layer.
Style the lines with a color and weight that make it stand out on all maps are also passed.
The tectonic layer group variable that is created in Step 1 to the map, i.e., .addTo(tectonicPlates) and close the geoJSON() layer is also added.
Tectonic layer group variable to the map, i.e, tectonicPlates.addTo(map) is added.
using live server following map is shown
![earthquake map pic](https://user-images.githubusercontent.com/112978144/222538694-f5310235-c6b7-49c7-a428-de862e6c0389.png)


# Deliverable 2

.In Step 1, a third layer group variable for the major earthquake data is added.
In Step 2, a reference to the major earthquake data to the overlay object is added.
In Step 3, using the d3.json() callback method is used to make a call to the major earthquake data from the GeoJSON Summary Feed for M4.5+ EarthquakesLinks to an external site. for the Past 7 Days.
In Step 4, using the same parameters in the styleInfo() function that made a call to the getColor() and getRadius() functions.
In Step 5, getColor() function is used to use only three colors for the following magnitudes; magnitude less than 5, a magnitude greater than 5, and a magnitude greater than 6.
In Step 6, using the same parameters from the preceding step in the getRadius() function.
In Step 7, passed the major earthquake data into the GeoJSON layer and do the following with the geoJSON() layer:
Turned each feature into a circleMarker on the map
Styled each circle with styleInfo() function
Created a popup for the circle to display the magnitude and location of the earthquake
Added the major earthquake layer group variable created in Step 1 to the map, i.e., .addTo(majorEQ) and then closed the geoJSON() layer.
Then, added the major earthquake layer group variable to the map, i.e, majorEQ.addTo(map), and then close the d3.json() callback.
live server shows this map

![image](https://user-images.githubusercontent.com/112978144/222538881-4d4d7930-f374-445a-9620-66bdd0dd4db7.png)

# Deliverable 3
Using knowledge of JavaScript and Leaflet.js added a third map style to the earthquake map.

Using the options from the Mapbox stylesLinks to an external site., added a third map style as a tile layer object to the challenge_logic.js file.
Added the map variable to the base layer object.

![image](https://user-images.githubusercontent.com/112978144/222539097-fd80b71c-4753-4029-8140-0ba467f57dc4.png)

# purpose 
This interactive map is created to help data reporters, analysts, and individuals visually identify trends in disasters and disaster reporting. The differences in magnitudes of earthquakes all over the world can be checked through popups used in the map.


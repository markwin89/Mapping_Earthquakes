# Mapping_Earthquakes

## Overview
### Purpose
To create a map that reflects earthquake data, tectonic plates locations, and areas that had a magnitude greater than 4.5.  Each with their own overlay and map that can be turned off or on. 

## Process 
### 3 Tile layers for the background view of the map. 
  - Added the mapbox tile layer for 3 different types of view: streets, satellite-streets, and dark. 
![Tile Layers](https://user-images.githubusercontent.com/101272613/175338569-9b321250-05e5-4a26-8367-59f289e95dd1.PNG)


### Map Object, Base Layers, Layer Groups, and Overlays.
  - Created the map object and default layer to have a set view when the local site is loaded. 
  - Added the base layer to hold 3 maps.
  - Added the 3 layer groups. 
  - Added the reference titles from the variables.  
![Base LayerGroup overlays mapobject](https://user-images.githubusercontent.com/101272613/175338628-400d290f-4308-43ed-b293-5ee5eaf60a0b.PNG)
![Dark tile](https://user-images.githubusercontent.com/101272613/175345332-970fb81d-6cd2-499f-8669-2cd2285e930f.PNG)
![Satelite tile](https://user-images.githubusercontent.com/101272613/175345363-02e75eac-f587-4317-b57d-7a79ea4b0d8e.PNG)

### GeoJSON Data and Color Properties.
  - Pulling the GeoJSON earthquake data.  
  - Created a function for radius and color that is dependent on the size of the magnitude.
![Color properties Data](https://user-images.githubusercontent.com/101272613/175339842-3945a7be-424a-42df-a41f-79a03d81f9fd.PNG)
  - Created a GeoJSON layer for circle markers with city and earthquake info when hovering over. 
  - Added the 2 layer (allEarthquake and tectonicPlates) to the map.
![Color properties Data for earthquakes and tectonic plates](https://user-images.githubusercontent.com/101272613/175339854-0e1f5fa9-b69d-45f9-888a-fffbab42d9a9.PNG)
  - Pulling the GeoJSON earthquakes that are greater than 4.5 magnitudes. 
  - Created a function for radius and color that is dependent on the size of the magnitude.
![Color Prop mag 4 5 data](https://user-images.githubusercontent.com/101272613/175342269-f64e8a90-22b2-4eb0-ab06-58958eeebd33.PNG)
  - Finalized the logic with legend function and Tectonic Plate line.
    - Added the colors for each level of magnitude.
    - Looped the function where the color square has a number label for each interval.
    - Created a call to retreive the data for tectonic plate outline.
![Legend and Tectonic Plate boundary call](https://user-images.githubusercontent.com/101272613/175343211-9bb6c9a6-e5cf-4872-bf02-db892c0e9dd8.PNG)

## Results
### Interactive Map
  - Map has multiple layers with the use of radio buttons
  - The 3 datasets can populate over each other or singled out.  
![Interactive Map](https://user-images.githubusercontent.com/101272613/175344851-9e9e9ec2-300c-4dd1-a895-5efba1e98305.png)




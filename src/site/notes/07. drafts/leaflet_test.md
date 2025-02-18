---
{"dg-publish":true,"permalink":"/07-drafts/leaflet-test/"}
---


> [!NOTE]- Quick Calculator  
> Map Height in Pixels: `INPUT[number:map_height_y]`  
> Map Width in Pixels: `INPUT[number:map_width_x]`  
> lat: `VIEW[{map_height_y} / 2][math]`  
> long: `VIEW[{map_width_x} / 2][math]`  
> How Many Pixels In Scale: `INPUT[number:scale_pixels]`  
> How Many Units in Scale: `INPUT[number:scale_pixels_range]`  
> Scale: `VIEW[1/({scale_pixels}/{scale_pixels_range})][math:mapCalc1]`

```leaflet  
id: Meridian1932
image: [[map_meridian_full.png]]
bounds: [[0,0], [5000, 5000\|0,0], [5000, 5000]]
height: 500px
width: 90%
lat: 2500
long: 2500
minZoom: -3
maxZoom: 0
defaultZoom: -1.5
zoomDelta: 0.5
unit: mi
scale: 0.09328358208955223
recenter: false
darkmode: false

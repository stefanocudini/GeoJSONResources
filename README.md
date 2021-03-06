# geojson-resources

Usable static GeoJSON resources simply.

## Install

```
npm i geojson-resources
```

## Usage

Loading by JQuery and show in Leaflet map directly in your page:
```javascript

//your map
var map = L.map(...);

$.when($.getJSON('https://unpkg.com/geojson-resources@1.1.0/world.json'))
.then(function(json) {
  
  //load world boundaries in your map
  L.geoJSON(json).addTo(map);
  
});
```

## Roadmap
* include other simple geometries
* organize each geometry hierarchically
* consider various levels of accuracy
* define a unique namespace for each resource

## License
This work is licensed under a **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License**. 

![Creative Commons License Logo](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png "License")

# GIS-portal
<H1> Web GIS development </H1>


# Getting start with this project

1. Download and install the geoserver. [Installation tutorial](https://docs.geoserver.org/stable/en/user/installation/win_binary.html).
2. Upload data to the geoserver. [data upload guide](https://youtu.be/vL6kgJmOCxg).
3. Change the [lib/js/layers.js](https://github.com/iamtekson/GIS-portal/blob/main/lib/js/layers.js) file according to your need. Below is the example of `layers.js` file,

```js
var layersFromGeoserver = [
  {
    layerName: "gis:BU_2020", // This is the layer name from geoserver
    layerTitle: "Building", // This name will be shown in the left-sidebar
    defaultCheck: "false", // The layer default visibility
    thumbnailUrl: "./img/bu_2020.PNG", //Thumbnail of the layer
    description: // Short description for the layer
      "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima nobis soluta molestiae asperiores quae! Veritatis",
  },

  {
    layerName: "gis:LP_2020",
    layerTitle: "Land parcel",
    defaultCheck: "checked",
    thumbnailUrl: "./img/lp_2020.PNG",
    description:
      "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima nobis soluta molestiae asperiores quae! Veritatis",
  },
]
```

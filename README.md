OGC Simple Geometry for ArcGIS JavaScript API
=============================================

This library adds support for conversion between [OGC Simple Geometry] and [ArcGIS Server API for Javascript geometry].

## Note ##

Esri now has their own OGC WKT parsing library, [Terraformer.WKT]. You may want to use that instead. (Terraformer did not exist when this project was created.)

We have not done any tests to see which WKT parsing library is fastest. If you do any tests, please [contact us via the issues section](https://github.com/WSDOT-GIS/ogcsimplegeometry/issues) and let us know the results.

## Usage ##
See the [test application](https://github.com/WSDOT-GIS/ogc-simple-geometry-test) for example usage.

## Supported ##

* Well-Known Text definitions

### Geometry Types ###

* POINT
* MULTIPOINT
* LINESTRING
* MULTILINESTRING
* POLYGON


## Sample ##
The sample application can be viewed at http://wsdot-gis.github.io/ogc-simple-geometry-test/.

## License ##
Licensed under [The MIT License](http://opensource.org/licenses/MIT).

## Files ##

### `SimpleGeometry.js` ###
This file defines the SimpleGeometry class / module.

### `ogcSimpleGeometry.vsdoc.js` ###
This file provides code completion for `ogcSimpleGeometry.js` in Visual Studio.  It does not actually provide any functionality and should not be referenced by HTML.

### `SimpleGeometryArcGis.js` ###
This module is used to convert `SimpleGeometry` objects into objects that can converted to [esri/geometry/Geometry] objects using the [esri/geometry/jsonUtils.fromJson] function

[ArcGIS Server API for Javascript geometry]:http://developers.arcgis.com/en/javascript/jsapi/geometry-amd.html
[esri/geometry/Geometry]:https://developers.arcgis.com/en/javascript/jsapi/geometry-amd.html
[esri/geometry/jsonUtils.fromJson]:https://developers.arcgis.com/en/javascript/jsapi/namespace_geometry-amd.html#fromJson
[OGC Simple Geometry]:http://www.opengeospatial.org/standards/sfa
[Terraformer.WKT]:http://terraformer.io/wkt-parser/

# @turf/length

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## length

Takes a [GeoJSON](http://geojson.org/geojson-spec.html#geojson-objects) and measures its length in the specified units, [Point]((Multi)Point)'s distance are ignored.

**Parameters**

-   `geojson` **[GeoJSON](http://geojson.org/geojson-spec.html#geojson-objects)** GeoJSON to measure
-   `options` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** Optional parameters (optional, default `{}`)
    -   `options.units` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** can be degrees, radians, miles, or kilometers (optional, default `kilometers`)

**Examples**

```javascript
var line = turf.lineString([[115, -32], [131, -22], [143, -25], [150, -34]]);
var length = turf.length(line, {units: 'miles'});

//addToMap
var addToMap = [line];
line.properties.distance = length;
```

Returns **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** length of GeoJSON

<!-- This file is automatically generated. Please don't edit it directly:
if you find an error, edit the source file (likely index.js), and re-run
./scripts/generate-readmes in the turf project. -->

---

This module is part of the [Turfjs project](http://turfjs.org/), an open source
module collection dedicated to geographic algorithms. It is maintained in the
[Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create
PRs and issues.

### Installation

Install this module individually:

```sh
$ npm install @turf/length
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```
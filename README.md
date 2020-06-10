## array-unsort

[![NPM package][npm-img-array-unsort]][npm-url-array-unsort]
[![Build Size][build-size-img-array-unsort]][build-size-url-array-unsort]

This **`npm`** module shuffles an arbitrary array. The module offers two methods: **`unsort`** method shuffles and returns a copy of the input array using the **Fisher-Yates** algorithm. The **`unsortInplace`** method unsorts the input array in-place and uses a modified Fisher-Yates method which guarantees that no array element remain at the same index after shuffling.

Module on `npm` [here](https://www.npmjs.com/package/array-unsort), repo [here](https://github.com/boeric/array-unsort)

Demo [here](https://bl.ocks.org/boeric/35eec347e240c6e41ebe04d85e28de9d)

## array-correl

[![NPM package][npm-img-array-correl]][npm-url-array-correl]
[![Build Size][build-size-img-array-correl]][build-size-url-array-correl]

This **`npm`** module generates random values with a specified correlation. It also allows inspection of an array to determine correlation between the array's values. The **`generate`** method takes the inputs count, desired correlation, mean and deviation and generates an array that satisfies the input parameters. The **`inspect`** method accepts an array, inspects the array and provides several statistics such as correlation coefficient, deviation, mean and extent (min, max).

Module on `npm` [here](https://www.npmjs.com/package/array-correl), repo [here](https://github.com/boeric/array-correl)

## license-suspensions

The visualization demonstrates how to syncronize the state of two side-by-side Mapbox GL based maps. As the user interacts with one of the two maps, the state of the map (center position, zoom level, pitch and bearing) is dynamically copied to the second map (and vice versa). The code also demonstrates how to prevent call stack overflow due to recursive event handler triggering when the map state is updated.

The project was made for the East Bay Community Law Center's **Back on the Road** initiative. The initiative's purpose was to highlight injustices in how driver licenses were suspended for failure to appear in court or failure to pay traffic tickets. As the visualization shows, there is significant correlation between driver license suspensions and poverty level 

The dataset is based on driver license suspensions from California DMV and East Bay Community Law Center. See the initiative description [here](https://ebclc.org/backontheroad/problem/)

See the project live [here](https://boeric.github.io/license-suspensions/), repo [here](https://github.com/boeric/license-suspensions)

## vertex-generator

The Vertex Generator allows rapid capture of verticies of a simulated path of a vechicle or person. Each captured vertex is a geo location where the path is changing direction. Each vertex also has a notion of speed. The geo locations and speed information can be used by a post processing tool to "fill in" the geo location between the verticies.

## geo-buffer

Creates "buffers" of arbitrary size around parks in San Francisco, using Mapbox Gl and Turf.js. Each GeoJson object (SF park) is "enlarged" with the value (in meters) of the input range control. The visualization demonstrates how overlapping GeoJson objects can be merged. Please note: the polygon merge process is currently unoptimized (meaning, for example, that each polygon is unnecessarily tested for overlap against all others), and will be improved by quad trees.

See the project live [here](https://boeric.github.io/geo-buffer/), repo [here](https://github.com/boeric/geo-buffer)

## geo-locate 

The script generates latitude and longitude information for each item in the input array, using the Google geocoder

## canvas-in-svg

The visualization demonstrates the use of an embedded Canvas in an SVG element. While this example includes only a single SVG element, an embedded canvas may make sense when a number of SVG elements needs to be generated, with each requiring to render large datasets that would othwewise overwhelm the DOM.

In this example, up to 50,000 elements can be generated and visualized in the embedded canvas with no impact to the DOM (other than creating the canvas). Mouse hit detection of data elements is performed with a 4x4 pixel zone under the current mouse position. 

See the project live [here](http://boeric.github.io/canvas-in-svg/), repo [here](https://github.com/boeric/canvas-in-svg)

## timestamped-geo-points

Expands an array of geo vertices to timestamped geo points. Previously captured verticies (input file) indicate geo locations where a geo path is changing direction. For example, a vehicle's path along a road may be captured with a set of verticies, each of which indicate where the vechicle's path is changing direction. 

## real-time-chart

The real time chart is a resuable Javascript component that accepts real time data. The chart's time domain is moving with the passage of time, which means that any data placed in the chart eventually will age out and leave the chart. In addition to the main chart, the component also manages a "focus" window with a viewport (d3.brush) that can moved and sized to view an arbitrary portion of the time series data.

## shootings

The visualization is using data from www.shootingtracker.com and covers the period January 2013 through early December 2015. The event data (comprised of over 1000 shooting events) has been grouped into weeks.

## migrants

Slippy (zoomable/draggable) map and tile management, with data layer comprised of semitransparent circles. Also demonstrates an info overlay activated when the user is hovering over a data item.

## drag-and-drop





[npm-img-array-unsort]: https://img.shields.io/npm/v/array-unsort.svg
[npm-url-array-unsort]: https://npmjs.org/package/array-unsort
[build-size-img-array-unsort]: https://img.shields.io/bundlephobia/minzip/array-unsort.svg
[build-size-url-array-unsort]: https://bundlephobia.com/result?p=array-unsort

[npm-img-array-correl]: https://img.shields.io/npm/v/array-correl.svg
[npm-url-array-correl]: https://npmjs.org/package/array-correl
[build-size-img-array-correl]: https://img.shields.io/bundlephobia/minzip/array-correl.svg
[build-size-url-array-correl]: https://bundlephobia.com/result?p=array-correl

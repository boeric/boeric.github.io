## Demos

## array-unsort

[![NPM package][npm-img-array-unsort]][npm-url-array-unsort]
[![Build Size][build-size-img-array-unsort]][build-size-url-array-unsort]

This **`npm`** module unsorts (shuffles) an input array. The **`unsort`** method scrambles the input array and returns a new array. The **`unsortInplace`** method scrambles the input array in-place. Two algorithms are available: **Fisher-Yates** and **Modified Fisher-Yates**. The latter guarantees that no array element remain at the same array index after shuffling.

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

## css-combinator-demo

Demo of CSS selector **combinators** using only native DOM methods

See the project live [here](https://bl.ocks.org/boeric/780904f668c1e2f27cdac8aa011e45cb), repo [here](https://gist.github.com/boeric/780904f668c1e2f27cdac8aa011e45cb)

## css-box-model-demo

A demo of the **CSS Box Model**, using **`D3`**. The project demonstrates a bunch of things, for example: 
- The effects of margin, border, padding and inner content dimensions of the overall size of DOM elements
- The optional use of **Flexbox** in laying out elements
- How to calculate the full dimension of an element
- How to extract current inline styles of elements

See the project live [here](https://bl.ocks.org/boeric/cbb5b416091e74c70b8480e68b6d21e1), repo [here](https://github.com/boeric/css-box-model-demo)

## github-api-demo

Demos of how to access the Github API to obtain metadata about a users public Repos and Gists. In addition, it demos how to do this using only native DOM methods (as no external libraries are used). It does however use Bootstrap for some styling. Also demos **`async-await`** when using **`fetch`**.

See the project live [here](https://bl.ocks.org/boeric/4950f26655187c33bedba9728e98a3c2), repo [here](https://gist.github.com/boeric/4950f26655187c33bedba9728e98a3c2)

## geo-buffer

Creates "buffers" of arbitrary size around **`geojson`** polygons and multi-polygons, in this case parks in San Francisco, using **Mapbox Gl** and **Turf.js**. Each GeoJson object (SF park) is "enlarged" with the value (in meters) of the input range control. The visualization demonstrates how overlapping GeoJson objects can be merged. Please note: the polygon merge process is currently unoptimized (meaning, for example, that each polygon is unnecessarily tested for overlap against all others), and will be improved by quad trees.

See the project live [here](https://boeric.github.io/geo-buffer/), repo [here](https://github.com/boeric/geo-buffer)

## vertex-generator

The Vertex Generator allows rapid capture of verticies of a simulated path of a vechicle or person. Each captured vertex is a geo location where the path is changing direction. Each vertex also has a notion of speed. The geo locations and speed information can be used by a post processing tool to "fill in" the geo location between the verticies.

See the project live [here](https://boeric.github.io/vertex-generator/), repo [here](https://github.com/boeric/vertex-generator)

## geo-locate 

The script generates latitude and longitude information for each item in an input array, using the Google geocoder

Repo is [here](https://github.com/boeric/GeoLocate)

## real-time-chart-multi

The **`real-time-chart-multi`** project is a resuable Javascript component that accepts real time data from **multiple** data streams. The purpose is to show the arrival time of real time events (or lack thereof), piped to the browser (for example via Websockets). Various attributes of each event can be articulated using **size**, **color** and **opacity** of the object generated for the event. 

See the project live [here](http://boeric.github.io/d3RealTimeChartMulti/). **Please wait for 30 sec** to see events from the 2nd data stream

Repo is [here](https://github.com/boeric/d3RealTimeChartMulti)

## real-time-chart

Similar to **`real-time-chart-multi`** (see above), but manages a single data stream.

See the project live [here](http://boeric.github.io/d3RealTimeChart/)

Repo is [here](https://github.com/boeric/d3RealTimeChart)

## canvas-in-svg

The visualization demonstrates the use of an embedded Canvas in an SVG element. While this example includes only a single SVG element, an embedded canvas may make sense when a number of SVG elements needs to be generated, with each requiring to render large datasets that would othwewise overwhelm the DOM.

In this example, up to 50,000 elements can be generated and visualized in the embedded canvas with no impact to the DOM (other than creating the canvas). Mouse hit detection of data elements is performed with a 4x4 pixel zone under the current mouse position. 

See the project live [here](http://boeric.github.io/canvas-in-svg/), repo [here](https://github.com/boeric/canvas-in-svg)

## timestamped-geo-points

Expands an array of geo vertices to timestamped geo points. Previously captured verticies (input file) indicate geo locations where a geo path is changing direction. For example, a vehicle's path along a road may be captured with a set of verticies, each of which indicate where the vechicle's path is changing direction. 

Repo is [here](https://github.com/boeric/timestamped-geo-points)

## shootings

The visualization is a demo of a 'slippy' (zoomable/draggable) map, using data from www.shootingtracker.com and covers the period January 2013 through early December 2015. The event data (comprised of over 1000 shooting events) has been grouped into weeks.

See the project live [here](http://bl.ocks.org/boeric/c1fe5650da3d6e790706), repo [here](https://github.com/boeric/shootings)

## migrants

Slippy (zoomable/draggable) map and tile management, with data layer comprised of semitransparent circles. Also demonstrates an info overlay activated when the user is hovering over a data item.

See the project live [here](http://bl.ocks.org/boeric/47aceae44bb5f8b63d7b), repo [here](https://github.com/boeric/migrants)

## drag-and-drop

Demo of drag and drop using only native HTML5 DOM methods.

See the project live [here](https://github.com/boeric/drag-and-drop), repo [here](https://bl.ocks.org/boeric/deb4dfb7bc6f1f9e9a5b3bdd4ad2cc2c)

[npm-img-array-unsort]: https://img.shields.io/npm/v/array-unsort.svg
[npm-url-array-unsort]: https://npmjs.org/package/array-unsort
[build-size-img-array-unsort]: https://img.shields.io/bundlephobia/minzip/array-unsort.svg
[build-size-url-array-unsort]: https://bundlephobia.com/result?p=array-unsort

[npm-img-array-correl]: https://img.shields.io/npm/v/array-correl.svg
[npm-url-array-correl]: https://npmjs.org/package/array-correl
[build-size-img-array-correl]: https://img.shields.io/bundlephobia/minzip/array-correl.svg
[build-size-url-array-correl]: https://bundlephobia.com/result?p=array-correl

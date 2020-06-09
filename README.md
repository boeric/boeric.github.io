## license-suspensions

The visualization demonstrates how to syncronize the state of two side-by-side Mapbox GL based maps. As the user interacts with one of the two maps, the state of the map (center position, zoom level, pitch and bearing) is dynamically copied to the second map (and vice versa). The code also demonstrates how to prevent call stack overflow due to recursive event handler triggering when the map state is updated.

The project was made for the East Bay Community Law Center's **Back on the Road** initiative. The initiative's purpose was to highlight injustices in how driver licenses were suspended for failure to appear in court or failure to pay traffic tickets. As the visualization shows, there is significant correlation between driver license suspensions and poverty level 

The dataset is based on driver license suspensions from California DMV and East Bay Community Law Center. See the initiative description [here](https://ebclc.org/backontheroad/problem/)

See the project live [here](https://boeric.github.io/license-suspensions/), repo [here](https://github.com/boeric/license-suspensions)
## geo-buffer

Creates "buffers" of arbitrary size around parks in San Francisco, using Mapbox Gl and Turf.js. Each GeoJson object (SF park) is "enlarged" with the value (in meters) of the input range control. The visualization demonstrates how overlapping GeoJson objects can be merged. Please note: the polygon merge process is currently unoptimized (meaning, for example, that each polygon is unnecessarily tested for overlap against all others), and will be improved by quad trees.

See the project live [here](https://boeric.github.io/geo-buffer/), repo [here](https://github.com/boeric/geo-buffer)

## canvas-in-svg

The visualization demonstrates the use of an embedded Canvas in an SVG element. While this example includes only a single SVG element, an embedded canvas may make sense when a number of SVG elements needs to be generated, with each requiring to render large datasets that would othwewise overwhelm the DOM.

In this example, up to 50,000 elements can be generated and visualized in the embedded canvas with no impact to the DOM (other than creating the canvas). Mouse hit detection of data elements is performed with a 4x4 pixel zone under the current mouse position. 

See the project live [here](http://boeric.github.io/canvas-in-svg/), repo [here](https://github.com/boeric/canvas-in-svg)

## array-unsort

[![NPM package][npm-img]][npm-url]
[![Build Size][build-size-img]][build-size-url]

This **`npm`** module shuffles an arbitrary array. The module offers two methods: **`unsort`** method shuffles and returns a copy of the input array using the **Fisher-Yates** algorithm. The **`unsortInplace`** method unsorts the input array in-place and uses a modified Fisher-Yates method which guarantees that no array element remain at the same index after shuffling.

[npm-img]: https://img.shields.io/npm/v/array-unsort.svg
[npm-url]: https://npmjs.org/package/array-unsort
[build-size-img]: https://img.shields.io/bundlephobia/minzip/array-unsort.svg
[build-size-url]: https://bundlephobia.com/result?p=array-unsort

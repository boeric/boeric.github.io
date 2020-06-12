## Demos

## array-unsort

[![NPM package][npm-img-array-unsort]][npm-url-array-unsort]
[![Build Size][build-size-img-array-unsort]][build-size-url-array-unsort]

This **npm** module unsorts (shuffles) an arbitrary array. The **unsort** method scrambles the input array and returns a new array. The **unsortInplace** method scrambles the input array in-place. Two algorithms are available: **Fisher-Yates** and **Modified Fisher-Yates**. The latter guarantees that no array element remain at the same array index after shuffling.

The module on **npm** [here](https://www.npmjs.com/package/array-unsort), repo [here](https://github.com/boeric/array-unsort)

Demo [here](https://bl.ocks.org/boeric/35eec347e240c6e41ebe04d85e28de9d)

## array-correl

[![NPM package][npm-img-array-correl]][npm-url-array-correl]
[![Build Size][build-size-img-array-correl]][build-size-url-array-correl]

This **npm** module generates random values with a specified correlation. It also allows inspection of an array to determine correlation between the array's values. The **generate** method takes the inputs count, desired correlation, mean and deviation and generates an array that satisfies the input parameters. The **inspect** method inspects an array and provides several statistics, such as correlation coefficient, deviation, mean and extent (min, max).

The module on **npm** [here](https://www.npmjs.com/package/array-correl), repo [here](https://github.com/boeric/array-correl)

## license-suspensions

The visualization demonstrates how to syncronize the state of two side-by-side MapboxGL-based maps. As the user interacts with one of the two maps, the state of the map (center position, zoom level, pitch and bearing) is dynamically copied to the second map (and vice versa). The code also demonstrates how to prevent call stack overflow due to recursive event handler triggering when the map state is updated.

<img src="https://user-images.githubusercontent.com/4840824/84468972-d7fa3f80-ac34-11ea-9d0a-b29c5d749c0e.png" width="700"/>

The project was made for the East Bay Community Law Center's **Back on the Road** initiative. The initiative's purpose was to highlight injustices in how driver licenses were suspended for failure to appear in court or failure to pay traffic tickets. As the visualization shows, there is significant correlation between driver license suspensions and poverty level 

The dataset is based on driver license suspensions from California DMV and East Bay Community Law Center. See the initiative description [here](https://ebclc.org/backontheroad/problem/)

See the project live [here](https://boeric.github.io/license-suspensions/), repo [here](https://github.com/boeric/license-suspensions)

## geo-buffer

Creates "buffers" of arbitrary size around **geojson** polygons and multi-polygons, in this case parks in San Francisco. It is using **MapboxGL** and **Turf**. Each GeoJson object (SF park) is "enlarged" with the value (in meters) of the input range control. The visualization demonstrates how overlapping GeoJson objects can be merged. 

<img src="https://user-images.githubusercontent.com/4840824/84538126-fa787100-aca5-11ea-831c-7768301435f7.png" width="500"/>

**Please note**: the polygon merge process is currently unoptimized (meaning, for example, that each polygon is unnecessarily tested for overlap against all others), and will be improved by quad trees.

See the project live [here](https://boeric.github.io/geo-buffer/), repo [here](https://github.com/boeric/geo-buffer)

## vertex-generator

The vertex generator allows rapid capture of geo verticies of a simulated path of a vechicle or person. Each captured vertex is a geo location where the path is changing direction. A syntactically valid **GeoJSON** structure is produced when the button is clicked. The GeoJSON structure contains both the **Point**s and **LineString** elements.  

<img src="https://user-images.githubusercontent.com/4840824/84546165-8645c980-acb5-11ea-8598-6589d925b6c3.png" width="500"/>

The geo locations and speed information can be used by a post processing tool to "fill in" the geo location between the verticies.

See the project live [here](https://boeric.github.io/vertex-generator/), repo [here](https://github.com/boeric/vertex-generator)

## timestamped-geo-points

Expands an array of geo vertices to timestamped geo points. Previously captured verticies (input file) indicate geo locations where a geo path is changing direction. For example, a vehicle's path along a road may be captured with a set of verticies, each of which indicate where the vechicle's path is changing direction. 

Repo is [here](https://github.com/boeric/timestamped-geo-points)

## real-time-chart-multi

The **real-time-chart-multi** project is a resuable Javascript component that accepts real time data from **multiple** data streams. The purpose is to show the arrival time of real time events (or lack thereof), piped to the browser (for example via Websockets). Various attributes of each event can be articulated using **size**, **color** and **opacity** of the object generated for the event. 

See the project live [here](http://boeric.github.io/d3RealTimeChartMulti/). **Please wait for 30 sec** to see events from the 2nd data stream

Repo is [here](https://github.com/boeric/d3RealTimeChartMulti)

## canvas-in-svg

The visualization demonstrates the use of an embedded Canvas in an SVG element. While this example includes only a single SVG element, an embedded canvas may make sense when a number of SVG elements needs to be generated, with each requiring to render large datasets that would othwewise overwhelm the DOM.

In this example, up to 50,000 items can be generated and visualized in the embedded canvas with no impact to the DOM (other than creating the canvas). Mouse hit detection of data elements is performed with a 4x4 pixel zone under the current mouse position. 

See the project live [here](http://boeric.github.io/canvas-in-svg/), repo [here](https://github.com/boeric/canvas-in-svg)

## shootings

The visualization is a demo of a slippy (zoomable/draggable) map, using data from www.shootingtracker.com and covers the period January 2013 through early December 2015. The event data (comprised of over 1000 shooting events) has been grouped into weeks.

See the project live [here](http://bl.ocks.org/boeric/c1fe5650da3d6e790706), repo [here](https://github.com/boeric/shootings)

## migrants

Slippy (zoomable/draggable) map and tile management, with data layer comprised of semitransparent circles. Also demonstrates an info overlay activated when the user is hovering over a data item.

See the project live [here](http://bl.ocks.org/boeric/47aceae44bb5f8b63d7b), repo [here](https://github.com/boeric/migrants)

## drag-and-drop

Demo of drag and drop using only native HTML5 DOM methods.

See the project live [here](https://bl.ocks.org/boeric/deb4dfb7bc6f1f9e9a5b3bdd4ad2cc2c), repo [here](https://github.com/boeric/drag-and-drop)

## css-combinator-demo

Demo of CSS selector **combinators** using only native DOM methods.

See the project live [here](https://bl.ocks.org/boeric/780904f668c1e2f27cdac8aa011e45cb), repo [here](https://gist.github.com/boeric/780904f668c1e2f27cdac8aa011e45cb)

## css-box-model-demo

A demo of the **CSS Box Model**, using **D3**. The project demonstrates a bunch of things, for example: 
- The effects of margin, border, padding and inner content dimensions of the overall size of DOM elements
- The optional use of **Flexbox** in laying out elements
- How to calculate the full dimension of an element
- How to extract current inline styles of elements

See the project live [here](https://bl.ocks.org/boeric/cbb5b416091e74c70b8480e68b6d21e1), repo [here](https://github.com/boeric/css-box-model-demo)

## github-api-demo

Demos of how to access the Github API to obtain metadata about a users' public Repos and Gists. In addition, it demos how to do this using only native DOM methods (as no external libraries are used). It does however use Bootstrap for some styling. Also demos **async-await** when using **fetch**.

See the project live [here](https://bl.ocks.org/boeric/4950f26655187c33bedba9728e98a3c2), repo [here](https://gist.github.com/boeric/4950f26655187c33bedba9728e98a3c2)

## infinite-scroll

React demo of inifite scroll of images from the **cat.api** where only a finite number of images are kept in the browser.

See the project live [here](http://demo.boe.net:8080/), repo [here](https://github.com/boeric/infinite-scroll)

## traffic-fines

Interactive map that shows traffic fines across the US. The visualization was created for the Laywers' Committee for Civil Rights of the San Francisco Bay Area. The user can select one of three data series (Fines for Redlight, Stop sign and Speeding violations). By hovering over a state, an overlay shows the specific data to that state. As the user is moving the mouse over the map, the legend at the bottom shows each state's position.

See the project live [here](https://www.lccr.com/programs/paying-poor-bias-disparity-californias-traffic-court-system/) (please scroll down to the map), repo [here](https://github.com/boeric/traffic-fines)

## event-hub

The event-hub project demonstrates how to create a central event dispatcher in a web application. The system is comprised of three main components: a) server, b) client web app, c) analytics web app

<img src="https://user-images.githubusercontent.com/4840824/84465018-dc215f80-ac2a-11ea-972f-20849fbb15fa.png" width="700"/>

The **server** is a combined **HTTP** and **Websockets** server. It delivers the required HTML files and related dependencies (assets and scripts). It also establishes a Websockets listener and dispatcher of Websockets messages. The server maintains a default configuration for event handling for each **client**. The server forwards to the **analytics** app the event summary messages produced by the **client** app. It also forwards configuration messages from the **analytics** app to the **client** app. 

**Please note** that there may be multiple instances of **client** and **analytics** web apps, doesn't matter – all information is distributed to the **full ecosystem** of attached apps using **Websockets**.

The **Client**, more specifically the **eventhub** is the most interesting piece of the project. The client loads an image with some buttons. Two scripts are used, the **eventhub** and **events**. The former is an event tracker/consolidator/forwarder, and the latter is an event generator. 

The event manager **eventhub.js** upon init, first checks for Websockets support (and terminates if no such support is available). It then attempts to establish communication with the **server** over Websockets and sets an event handler for incoming Websockets messages. It then adds the **eventhub** function to the **window** object, making it available to all scripts running in the browser.

Run the **client** web app [here](http://demo.boe.net:5000/). Then in a separate window, run the **analytics** web app [here](http://demo.boe.net:5000/analytics). Then trigger events in the **client** (by moving the mouse) and watch the events being consolidated and forwarded to the **analytics** app

Repo not yet published

## sensor-vue

The sensor-vue project is a full stack implementation of:

1. Sensor software running on a dozen remote **Raspberry PIs**
2. An HTTP server implementation, using **Node** and **Express**
3. A **React** webapp to view the collected sensor data 

The Raspberry Pies are programmed to sample the various attached sensors (temperature, water, humidity and air pressure) every minute and to forward the collected data to the Server component (also every minute) via HTTP. 

A **flow control protocol** is implemented between the pies and the server to eliminate any chance that the server becomes overloaded after a long server outage. In essence, the following occurs at every upload moment:

1. The pie tells the server how many data packets are contained in the pie's data buffer. Normally that would be one packet, but after a server outage, the pie's buffer will contain a number of packets equal to the server's (or communication link) outage in minutes
2. The server **directs** the pie to send either all packets or a subset of the packets that may have stacked up
3. The pie sends the number of packets it is **allowed** to send, in FIFO order
4. The server stores the packets in a DB (currently file system)
5. At each upload moment, the server directs the pie to **update its internal clock** to the time provided by the server, which is set to **UTC**
6. While each pie is sampling its sensors and sends the data every minute to the server (as outlined above), to avoid that the server is hit simultaneously by all sensors attempting to push the latest data, there is a time offset in seconds from the beginning of the minute determined by the last nibble in the pie's MAC address (time dithering).

In addition to the sensor data embedded in the data payload, a number of other values are provided in the payload, such the sequence number (which increments every minute), the current wifi link quality and bitrate, the uptime, the current temperature of the CPU, and sweep time (the time from probing the first sensor attached to the pie to obtaining the result from the last sensor)

The server also delivers the React web application on demand. The server and web app use **Websockets** for real time transmission of received sensor data to the web app. The server is also providing an **API** which the web app uses to retrieve non-real-time data

The system has been operational since 2017 and **no data packets have been lost** other than during power outage at the sensor locations. As of June 2020, the sensors have each delivered over **1.5 million packets** to the server. Some pies died however, probably due to failure of the flash memory cards.

Open the screenshot below in **another browser window** to see image details.

<img src="https://user-images.githubusercontent.com/4840824/84548914-9a8cc500-acbb-11ea-8161-470bd1d5695c.png" width="700"/>

**Please note**: Login is required to see sensor status

See the project live [here](http://www.sensorvue.com)

Repo not yet published

[npm-img-array-unsort]: https://img.shields.io/npm/v/array-unsort.svg
[npm-url-array-unsort]: https://npmjs.org/package/array-unsort
[build-size-img-array-unsort]: https://img.shields.io/bundlephobia/minzip/array-unsort.svg
[build-size-url-array-unsort]: https://bundlephobia.com/result?p=array-unsort

[npm-img-array-correl]: https://img.shields.io/npm/v/array-correl.svg
[npm-url-array-correl]: https://npmjs.org/package/array-correl
[build-size-img-array-correl]: https://img.shields.io/bundlephobia/minzip/array-correl.svg
[build-size-url-array-correl]: https://bundlephobia.com/result?p=array-correl

## Demos

## array-correl

[![NPM package][npm-img-array-correl]][npm-url-array-correl]
[![Build Size][build-size-img-array-correl]][build-size-url-array-correl]

The **npm** module generates an array of arbitrary size of pairs of numbers with a specified correlation. It also allows inspection of such array to determine the **pearson** correlation coefficient of the array's value pairs. The **generate** method takes the input count (array length), desired correlation, mean and deviation, and from this generates an array of numeric pairs that satisfies the input parameters. The **inspect** method inspects such array and provides several statistics, such as the actual pearson correlation coefficient, deviation, mean and extent. The only dependency is **d3-array** which could easily be factored away in a future version.

The module on **npm** [here](https://www.npmjs.com/package/array-correl)

The Repo is [here](https://github.com/boeric/array-correl)

Cool demo [here](https://bl.ocks.org/boeric/aa80b0048b7e39dd71c8fbe958d1b1d4)

## array-unsort

[![NPM package][npm-img-array-unsort]][npm-url-array-unsort]
[![Build Size][build-size-img-array-unsort]][build-size-url-array-unsort]

The **npm** module unsorts (shuffles) an arbitrary array. The **unsort** method scrambles the input array and returns a new array. The **unsortInplace** method scrambles the input array in-place. Two algorithms are available: **Fisher-Yates** and **Modified Fisher-Yates**. The latter guarantees that no array element remain at the same array index after shuffling.

The module on **npm** [here](https://www.npmjs.com/package/array-unsort)

The Repo is [here](https://github.com/boeric/array-unsort)

Demo [here](https://bl.ocks.org/boeric/35eec347e240c6e41ebe04d85e28de9d)

## zero-config-modern-webapp / zero-config-react-webapp (brand new)

Zero-config modern **Js** front-end or **React** web app templates, with Webpack (bundler), Babel (compiler), Eslint/Airbnb (strict code style linting), Jest (unit tests), and D3 (data visualization) – all **pre-configured** and ready to go. You just add your code! 

In development mode, the webapp (served on `localhost:8080`) will reload after each file save.

Also, these cool new/newish javascript features are enabled: async/await, spread, generators, Map/Set, WeakMap/WeakSet, getters/setters and optional chaining (`?.`) – and work in legacy browsers! 

The Javascript Repo is [here](https://github.com/boeric/zero-config-modern-webapp)

The React Repo is [here](https://github.com/boeric/zero-config-react-webapp)

## license-suspensions

The visualization demonstrates how to syncronize the state of two side-by-side **MapboxGL**-based maps. As the user interacts with one of the two maps, the state of the map (center position, zoom level, pitch and bearing) is dynamically copied to the second map (and vice versa). The code also demonstrates how to prevent call stack overflow due to recursive event handler triggering when the map state is updated.

<img src="https://user-images.githubusercontent.com/4840824/84468972-d7fa3f80-ac34-11ea-9d0a-b29c5d749c0e.png" width="700"/>

The project was made for the **East Bay Community Law Center**'s ["Back on the Road"](https://ebclc.org/backontheroad/problem/) initiative. The initiative's purpose was to highlight injustices in how driver licenses were suspended for failure to appear in court or failure to pay traffic tickets. As the visualization shows, there is significant correlation between driver license suspensions and poverty level 

The dataset is based on driver license suspensions from California DMV and East Bay Community Law Center. See the initiative [here](https://ebclc.org/backontheroad/problem/)

See the project live [here](https://boeric.github.io/license-suspensions/)

The repo is [here](https://github.com/boeric/license-suspensions)

## dataset-insights

The objective with this project is to provide **near-instanteous insights** of the contents of numeric columnar datasets. The following information is calculted for each numeric column in the dataset: null count, unique values (% of total values), extent (min/max), histogram and quantiles.

When a column is clicked, a red banner is shown on top of the column (please see screenshot below). Scatter plots of the **other** numeric columns are then generated (with x values from the column and y values from the selected column). The **pearson** correlation coefficent is calculated and displayed and a red line is drawn on top of the scatterplot with a slope equal to the correlation coefficient. The line's opacity is driven by the absolute value of the correlation coefficient.  

Open the screenshot below in **another browser window** to see image details.

<img src="https://user-images.githubusercontent.com/4840824/84852452-bd97db80-b011-11ea-8871-55dcb2ad689f.png" width="600"/>

See the project live [here](http://demo.boe.net/data-properties/)

Repo not yet published

## geo-buffer

Creates "buffers" of arbitrary size around **geojson** polygons and multi-polygons, in this case parks in San Francisco. It is using **MapboxGL** and **Turf**. Each GeoJson object (SF park) is "enlarged" with the value (in meters) of the input range control. The visualization demonstrates how overlapping GeoJson objects can be merged. 

<img src="https://user-images.githubusercontent.com/4840824/84538126-fa787100-aca5-11ea-831c-7768301435f7.png" width="500"/>

**Please note**: the polygon merge process is currently unoptimized (meaning, for example, that each polygon is unnecessarily tested for overlap against all others), and will be improved by quad trees.

See the project live [here](http://demo.boe.net/geo-buffer/){:target="_blank"}

The Repo is [here](https://github.com/boeric/geo-buffer)

## canvas-in-svg

The visualization demonstrates the use of an embedded Canvas in an SVG element. While this example includes only a single SVG element, an embedded canvas may make sense when a number of SVG elements needs to be generated, with each requiring to render large datasets that would othwewise overwhelm the DOM.

<img src="https://user-images.githubusercontent.com/4840824/84855916-2aaf6f00-b01a-11ea-89b7-2704f202f6ab.png" width="600"/>

In this implementation, up to 50,000 items can be generated and visualized in the embedded canvas with no impact to the DOM (other than creating the canvas). **Mouse hit detection** of data elements is performed with a **4x4** pixel zone under the current mouse position. 

The app is using the **array-correl** npm module referenced at the top

See the project live [here](http://demo.boe.net/canvas-in-svg/)

The Repo is [here](https://github.com/boeric/canvas-in-svg)

## d3-blocks

A variety of smaller projects, most of them using **D3**

<img src="https://user-images.githubusercontent.com/4840824/84855197-621d1c00-b018-11ea-9537-3356a878b35a.png" width="600"/>

See the Blocks [here](https://bl.ocks.org/boeric)

## infinite-scroll

**React app** demo of inifite scroll of images from the **cat.api** where only a finite number of images are kept in the browser. The project demonstrates loading resources **on-demand** during scrolling actions while keeping the browser **memory requirement** low. It also demonstrates how to keep the images in a **stable** position as the user is scrolling up/down using an API that provides **random** images.

The overlay window shows the currently visible images in **yellow** and the images kept in the browser in **gray**. 

<img src="https://user-images.githubusercontent.com/4840824/84854463-91328e00-b016-11ea-8c1d-9690615566b8.png" width="400"/>

See the project live [here](http://demo.boe.net:8080/)

The Repo is [here](https://github.com/boeric/infinite-scroll)

## traffic-fines

Interactive map that shows traffic fines across the US. The visualization was created for the **Laywers' Committee for Civil Rights** of the San Francisco Bay Area, to illustrate the high traffic fines in the state of California (please see screenshot) relative to other states. The user can select one of three data series (Fines for Redlight, Stop sign and Speeding violations). By hovering over a state, an overlay shows the specific data to that state. As the user is moving the mouse over the map, the legend at the bottom shows each state's position.

<img src="https://user-images.githubusercontent.com/4840824/84853807-dd7cce80-b014-11ea-9a7f-a7bb764ade79.png" width="600"/>

See the project live [here](https://www.lccr.com/programs/paying-poor-bias-disparity-californias-traffic-court-system/) (please scroll down to the map)

The Repo is [here](https://github.com/boeric/traffic-fines)

## network-viz

Network visualization of a simulated **compute infrastructure** with some 400 nodes/links in 3d using the **3d-force-graph** npm module. As can be seen from the viz, some segments are disconnected from core infrastructure. The viz provides insights into the topology of a network that would be difficult to obtain through any other means. 

<img src="https://user-images.githubusercontent.com/4840824/85204342-ba7a4500-b2c8-11ea-80dc-92283cf93989.png" width="700"/>

See the project live [here](http://demo.boe.net/network-viz/)

How to use: 
- Hover over a node to see the node details
- Select a node by clicking. The node's group is highlighted in the group list to the left
- Select a group by clicking in the group list to the left
- To select all nodes, click the Root group
- To zoom in/out, use the mouse wheel
- To rotate, drag with the left mouse button down
- To pan, drag with the right mouse button down

Repo not yet published

## point-cloud-deck-gl

Visualization of a "point cloud" using DeckGL and MapBoxGL. Close to 300k vertices are rendered above the map. The user can zoom in/out, rotate the map and change the pitch angle with the keyboard. 

<img src="https://user-images.githubusercontent.com/4840824/85961605-66263380-b960-11ea-8f86-e06571dc6f7b.png" width="700"/>

See the project live [here](http://demo.boe.net/point-cloud/)

Repo not yet published

## event-hub

The event-hub project demonstrates how to create a central event dispatcher in a web application. The system is comprised of three main components: 
- Server
- Client web app
- Analytics web app

<img src="https://user-images.githubusercontent.com/4840824/84465018-dc215f80-ac2a-11ea-972f-20849fbb15fa.png" width="700"/>

The **server** is a combined **HTTP** and **Websockets** server. It delivers the required HTML files and related dependencies (assets and scripts). It also establishes a Websockets listener and dispatcher of Websockets messages. The server maintains a default configuration for event handling for each **client**. The server forwards to the **analytics** app the event summary messages produced by the **client** app. It also forwards configuration messages from the **analytics** app to the **client** app. 

**Please note** that there may be multiple instances of **client** and **analytics** web apps, doesn't matter – all information is distributed to the **full ecosystem** of attached apps using **Websockets**.

The **Client**, more specifically the **eventhub** is the most interesting piece of the project. The client loads an image with some buttons. Two scripts are used, the **eventhub** and **events**. The former is an event tracker/consolidator/forwarder, and the latter is an event generator. 

The event manager **eventhub.js** upon init, first checks for Websockets support (and terminates if no such support is available). It then attempts to establish communication with the **server** over Websockets and sets an event handler for incoming Websockets messages. It then adds the **eventhub** function to the **window** object, making it available to all scripts running in the browser.

Run the **client** web app [in a separate window](http://demo.boe.net/event-hub/index.html). Then run the **analytics** web app [in another separate window](http://demo.boe.net/event-hub/analytics.html). Then trigger events in the **client** (by moving the mouse, clicking buttons, etc) and watch the events being consolidated and forwarded to the **analytics** app (via Websockets)

The Repo is [here](https://github.com/boeric/event-hub)

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

**Please note**: Login is required to see sensor status. However, in the debugger you can view the **realtime sensor data streaming over websockets**. 

See the project live [here](http://www.sensorvue.com)

Repo not yet published

## real-time-chart-multi

The **real-time-chart-multi** project is a resuable Javascript component that accepts real time data from **multiple** data streams. The purpose is to show the arrival time of real time events (or lack thereof), piped to the browser (for example via Websockets). Various attributes of each event can be articulated using **size**, **color** and **opacity** of the object generated for the event. 

<img src="https://user-images.githubusercontent.com/4840824/84856371-5c750580-b01b-11ea-88bc-f40714b1d5c9.png" width="600"/>

See the project live [here](http://boeric.github.io/d3RealTimeChartMulti/). **Please wait for 30 sec** to see events from the 2nd data stream

The Repo is [here](https://github.com/boeric/d3RealTimeChartMulti)

## vertex-generator

The vertex generator allows rapid capture of geo verticies of a simulated path of a vechicle or person. Each captured vertex is a geo location where the path is changing direction. A syntactically valid **GeoJSON** structure is produced when the button is clicked. The GeoJSON structure contains both the **Point**s and **LineString** elements.  

<img src="https://user-images.githubusercontent.com/4840824/84546165-8645c980-acb5-11ea-8598-6589d925b6c3.png" width="500"/>

The geo locations and speed information can be used by a post processing tool to "fill in" the geo location between the verticies.

To use, create vertexes in the map by clicking. Then click the **Get GEOJson** button, and copy the just-created GEOJson structure to the clipboard. Then drop it into for example [GeoJSONLint](https://geojsonlint.com/), to verify the integrity of the structure.

See the project live [here](https://boeric.github.io/vertex-generator/)

The Repo is [here](https://github.com/boeric/vertex-generator)

[npm-img-array-unsort]: https://img.shields.io/npm/v/array-unsort.svg
[npm-url-array-unsort]: https://npmjs.org/package/array-unsort
[build-size-img-array-unsort]: https://img.shields.io/bundlephobia/minzip/array-unsort.svg
[build-size-url-array-unsort]: https://bundlephobia.com/result?p=array-unsort

[npm-img-array-correl]: https://img.shields.io/npm/v/array-correl.svg
[npm-url-array-correl]: https://npmjs.org/package/array-correl
[build-size-img-array-correl]: https://img.shields.io/bundlephobia/minzip/array-correl.svg
[build-size-url-array-correl]: https://bundlephobia.com/result?p=array-correl

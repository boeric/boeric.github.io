## license-suspensions

The visualization demonstrates how to syncronize the state of two side-by-side Mapbox GL based maps. As the user interacts with one of the two maps, the state of the map (center position, zoom level, pitch and bearing) is dynamically copied to the second map (and vice versa). The code also demonstrates how to prevent call stack overflow due to recursive event handler triggering when the map state is updated.

The project was made for the East Bay Community Law Center's **Back on the Road** initiative. The initiative's purpose was to highlight injustices in how driver licenses were suspended for failure to appear in court or failure to pay traffic tickets. As the visualization shows, there is significant correlation between driver license suspensions and poverty level 

The dataset is based on driver license suspensions from California DMV and East Bay Community Law Center. See the initiative description [here](https://ebclc.org/backontheroad/problem/)

See the project live [here](https://boeric.github.io/license-suspensions/)
## geo-buffer

Creates "buffers" of arbitrary size around parks in San Francisco, using Mapbox Gl and Turf.js. Each GeoJson object (SF park) is "enlarged" with the value (in meters) of the input range control. The visualization demonstrates how overlapping GeoJson objects can be merged. Please note: the polygon merge process is currently unoptimized (meaning, for example, that each polygon is unnecessarily tested for overlap against all others), and will be improved by quad trees.

See the project live [here](https://boeric.github.io/geo-buffer/)



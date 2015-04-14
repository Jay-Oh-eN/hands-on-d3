# Hands on D3!

These are the materials for my workshop on creating interactive data visualization with D3!

I would love your feedback on the materials in the Github [issues](https://github.com/Jay-Oh-eN/hands-on-d3/issues).

And please do not hesitate to reach out to me directly via email at jondinu@gmail.com or over twitter @clearspandex


> Throughout this workshop, you will learn how to make this interactive parallel coordinate plot of environmental conditions related to incidences of Asthma in SF.

## Getting Setup

You will need:

* HTTP web server
    * On OSX and Linux `python -m SimpleHTTPServer`
    * On Windows, I recommend downloading [Mongoose][mongoose]
* Text Editor: I recommend [Sublime Text][sublime]
* A (modern) Web Browser: I recommend [Google Chrome][chrome]

Once you have downloaded the software above, you are ready to start making some data visualizations!

![](http://media2.giphy.com/media/rOTGSPxvJJY7m/giphy.gif)

1. Get the files: Download the [ZIP][zip] or `git clone https://github.com/Jay-Oh-eN/hands-on-d3.git` (git [tutorial][gitit]) this repository.
2. Start you HTTP web server
    * If using a `SimpleHTTPServer`, navigate into the repository folder (`hands-on-d3`) on your machine before you start the server.
    * If using Mongoose, set the 'Shared Directory' to be the repository folder.
3. Navigate with a web browser to `http://localhost:[port]` where [port] is the port the server has started on (`SimpleHTTPServer` defaults to port 8000)
4. You should see the directory listing, click on any of the `.html` files and you should see the charts.

__If you need some help with Javascript or D3, refer to the [tutorials](#resources) below__

### Libraries Used
* [D3.js][d3]
* [Parallel Coordinates][parallel]

## The Data

The [data][sf-asthma] is from the city of SF about certain environmental and health conditions of given Census tracts in the City.  You can read more about the individual fields from the [data dictionary][dictionary].

> This comprehensive dataset was used to inform and calculate the Heat Vulnerability Index for our Climate and Health Program. The dataset includes satellite imagery from NASA, temperature data from NOAA and other data sets such as individual physiology, culture, local infrastructure, behavior, and social and demographic characteristics which influence the risk of heat-related health impacts.

There 21 fields in the file (comma separated with headers) but we will be focusing on the following 8 fields:

<div class="output_subarea output_html rendered_html output_result"><div style="overflow:auto;">
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>AsthmaRates</th>
      <th>AirQuality</th>
      <th>SurfaceTemperature0908</th>
      <th>NonWhite</th>
      <th>Income</th>
      <th>NoHighSchoolDegree</th>
      <th>PopulationDensity</th>
      <th>TreeDensity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td> 6.299994</td>
      <td> 2.2</td>
      <td> 322</td>
      <td> 0.230650</td>
      <td>  93777</td>
      <td> 0.013605</td>
      <td>  1985.746482</td>
      <td> 1185</td>
    </tr>
    <tr>
      <th>1</th>
      <td> 6.276086</td>
      <td> 2.2</td>
      <td> 316</td>
      <td> 0.398085</td>
      <td>  73540</td>
      <td> 0.130243</td>
      <td> 27208.307880</td>
      <td> 6133</td>
    </tr>
    <tr>
      <th>2</th>
      <td> 5.700004</td>
      <td> 2.1</td>
      <td> 313</td>
      <td> 0.124894</td>
      <td> 171257</td>
      <td> 0.024085</td>
      <td>  7245.100198</td>
      <td> 2989</td>
    </tr>
    <tr>
      <th>3</th>
      <td> 5.699994</td>
      <td> 2.2</td>
      <td> 314</td>
      <td> 0.104333</td>
      <td> 187377</td>
      <td> 0.014402</td>
      <td> 41077.512777</td>
      <td> 5047</td>
    </tr>
    <tr>
      <th>4</th>
      <td> 5.699984</td>
      <td> 2.2</td>
      <td> 312</td>
      <td> 0.175050</td>
      <td> 117254</td>
      <td> 0.040223</td>
      <td> 21792.728792</td>
      <td> 3155</td>
    </tr>
    <tr>
      <th> ...</th>
      <td> ...</td>
      <td> ...</td>
      <td> ...</td>
      <td> ...</td>
      <td> ...</td>
      <td> ...</td>
      <td> ...</td>
      <td> ...</td>
    </tr>
  </tbody>
</table>
</div></div>

<hr>

## Visualization Examples

### Author Driven

#### [Facebook IPO][facebook] (NYT)

![][facebook_ipo_nyt]

#### [Syrian Refugee Crisis][syria] (Wesam Manassra)

![][syria-img]

### Viewer Driven

#### [Crimespotting][crimespotting] (Stamen)

![][crimespotting-screenshot]

### Martini Glass (mix of author and viewer)

#### [Visualizing MBTA Data][mbta] (Mike Barry and Brian Card)

![][mbta-img]

#### [Gun Deaths][guns] (Periscopic)

![][guns-img]

#### [Flight Delays][flights] (538)

![][flights-img]

## Next Steps
* [Visual Storytelling with D3 (Ritchie King)][ritchie]
* [Data Visualization and D3.js (Udacity)][udacity]
* [Interactive Data Vizualization (Scott Murray)][murray]
* [CSE512: Data Visualization (University of Washington)][uw-viz]
* [D3 Meetups][meetups]

## Resources

### General

* [A Tour Through the Visualization Zoo][zoo]

### Javascript
* [JS for Cats (beginner)][jscats]
* [Code School interactive][codeschool]
* [Eloquent Javascript (more advanced)][eloquent]
* [Superhero.js (set of resources)][supjs]

### D3
* [Let's Make a Bar Chart][barchart]
* [How Selections Work][selections]
* [Thinking with Joins][joins]
* [General Update Pattern][update]
* [Working with Transitions][transitions]
* [Gallery of D3 example][gallery]
* [Dashing D3][dashing]
* [D3 Noob][d3noob]
* [D3 Show Reel][showreel]
* [D3 master list of tutorials][tuts]
* [bl.ocksplorer][blocksplore]
* [Towards Reusable Charts][charts]

### D3 Libraries

* [RAW (GUI)][raw]
* [D3plus (charting)][d3plus]
* [Rickshaw (timeseries)][rickshaw]
* [dc.js (multidimensional)][dc.js]
* [NVD3 (charting)][nvd3]
* [c3.js (charting)][c3]
* [Queue.js (multiple data files)][queue]

## License

Copyright 2015 Jonathan Dinu.

All files and content licensed under [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License](LICENSE)

Rights of examples and screenshots of data visualizations belong to the authors themselves.

<!-- links -->

[mongoose]: http://cesanta.com/mongoose.shtml
[sublime]: http://www.sublimetext.com/2
[chrome]: https://www.google.com/chrome/browser/desktop/
[zip]: https://github.com/Jay-Oh-eN/hands-on-d3/archive/master.zip
[gitit]: http://jlord.us/git-it/
[mongoose-config]: images/mongoose-config.png

[sf-asthma]: https://data.sfgov.org/Health-and-Social-Services/Climate-and-Health-Data/paqg-zyqx
[grayarea]: http://grayarea.org/
[swiss]: http://www.swissnexsanfrancisco.org/
[lift]: http://liftconference.com/lift15
[data-canvas-img]: images/data-canvas.png
[data-canvas]: http://datacanvas.org/
[data-canvas-map]: http://map.datacanvas.org/
[dump]: https://s3.amazonaws.com/localdata-export/datacanvas/full.zip
[data-canvas-data]: http://map.datacanvas.org/#!/data
[dictionary]: data/dictionary.pdf

[d3]: http://d3js.org/
[dimple]: http://dimplejs.org/
[moment]: http://momentjs.com/
[d3plus]: http://d3plus.org/
[rickshaw]: http://code.shutterstock.com/rickshaw/
[dc.js]: http://dc-js.github.io/dc.js/
[nvd3]: http://nvd3.org/
[c3]: http://c3js.org/
[raw]: http://app.raw.densitydesign.org/
[queue]: https://github.com/mbostock/queue
[parallel]: https://syntagmatic.github.io/parallel-coordinates/

[crimespotting]: http://sanfrancisco.crimespotting.org/#zoom=13&lon=-122.438&types=AA,Mu,Ro,SA,DP,Na,Al,Pr,Th,VT,Va,Bu,Ar&lat=37.760&hours=0-23&dtend=2014-02-28T23:59:59-07:00&dtstart=2014-02-21T23:59:59-07:00
[crimespotting-screenshot]: images/crimespotting-screenshot.png
[facebook]: http://www.nytimes.com/interactive/2012/05/17/business/dealbook/how-the-facebook-offering-compares.html
[facebook_ipo_nyt]: images/facebook_ipo_nyt.png
[mbta]: http://mbtaviz.github.io/
[mbta-img]: images/mbta-img.png
[guns]: http://guns.periscopic.com/
[guns-img]: images/periscopic.png
[syria]: http://visualizations.manassra.com/syria
[syria-img]: images/syria-img.png
[final-viz]: images/animated_line.png
[viz-ani]: images/viz-ani.gif
[flights]: http://fivethirtyeight.com/interactives/flights/
[flights-img]: images/flights.png

[udacity]: https://www.udacity.com/course/ud507
[uw-viz]: http://courses.cs.washington.edu/courses/cse512/14wi/
[murray]: http://chimera.labs.oreilly.com/books/1230000000345
[ritchie]: http://ritchiesking.com/book/
[jscats]: http://jsforcats.com/
[eloquent]: http://eloquentjavascript.net/
[supjs]: http://superherojs.com/
[codeschool]: https://www.codeschool.com/paths/javascript
[barchart]: http://bost.ocks.org/mike/bar/
[d3noob]: http://www.d3noob.org/
[dashing]: https://www.dashingd3js.com/
[showreel]: http://bl.ocks.org/mbostock/1256572
[gallery]: https://github.com/mbostock/d3/wiki/Gallery
[tuts]: https://github.com/mbostock/d3/wiki/Tutorials
[joins]: http://bost.ocks.org/mike/join/
[selections]: http://bost.ocks.org/mike/selection/
[update]: http://bl.ocks.org/mbostock/3808218
[blocksplore]: http://bl.ocksplorer.org/
[transitions]: http://bost.ocks.org/mike/transition/
[zoo]: http://homes.cs.washington.edu/~jheer/files/zoo/
[meetups]: http://d3-js.meetup.com/
[charts]: http://bost.ocks.org/mike/chart/
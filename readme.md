# Hands on D3!

These are the materials for my workshop on creating interactive data visualization with D3!

I would love your feedback on the materials in the Github [issues](https://github.com/Jay-Oh-eN/hands-on-d3/issues).

And please do not hesitate to reach out to me directly via email at jondinu@gmail.com or over twitter @clearspandex

![Imgur](http://i.imgur.com/uNMk5Ch.gif)

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

### Whats in here?

    data/                data.sfgov.org datset on Climate and Health in SF
    images/              static image examples to be used in the readme.md
    lib/                 supporting JavaScript library files
    exercise_1.html      file containing dimple.js exercise
    exercise_2.html      D3 equivalent of dimple.js line chart
    exercise_3.html      animating line plot with interactive buttons
    LICENSE              Details of rights of use and distribution
    presentation.pdf     lecture slides from presentation
    readme.md            this file!
    template.html        HTML and Javascript scaffold to start from

## The Data

The [data][sf-asthma] is from the city of SF about certain environmental and health conditions of given Census tracts in the City.  You can read more about the individual fields from the [data dictionary][dictionary].

> This comprehensive dataset was used to inform and calculate the Heat Vulnerability Index for our Climate and Health Program. The dataset includes satellite imagery from NASA, temperature data from NOAA and other data sets such as individual physiology, culture, local infrastructure, behavior, and social and demographic characteristics which influence the risk of heat-related health impacts.

The files are comma separated with headers and 8 fields:

timestamp|city|temperature|light|airquality_raw|sound|humidity|dust
:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:
2015-02-16T17:00:00.000Z|San Francisco|20.8856185354523|2231.45801048026|28.8458008730416|1674.71050009727|48.4880466992298|882.367404134883
2015-02-16T18:00:00.000Z|San Francisco|21.8623045793052|2542.46720508251|26.5113633058142|1652.25960948903|43.9341875396295|912.0280753969
2015-02-16T19:00:00.000Z|San Francisco|23.5113166041101|3215.03460441893|24.8987852323788|1690.5842506536|40.5058249680354|939.447105875158
2015-02-16T20:00:00.000Z|San Francisco|25.6472096479114|4558.69142401972|26.0867059045864|1704.29832357106|38.4312464272035|999.743066983922

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
[zip]: https://github.com/Jay-Oh-eN/strata-interactive-data-viz/archive/master.zip
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
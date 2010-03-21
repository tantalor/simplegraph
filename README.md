# SimpleGraph

http://benaskins.github.com/simplegraph

## Description

Simple javascript graphs using Raphael and jQuery. 

Based on the Raphael [analytics example](http://raphaeljs.com/analytics.html) by Dmitry Baranovskiy 

## Usage

The SimpleGraph function takes four arguments:

 * __target:__ where the rendered graph will land
 * __data:__ an array of values to plot against the y-axis
 * __labels:__ an array of values for labelling the x-axis
 * __options:__ hash of options to customise the graph (see below)
  
### Simple example

    $("#myGraph").simplegraph([1,2,3,3,2,1], ["a","b","c","d","e","f"]);
  
Will render a graph that looks a little something like this (open `index.html` for actual rendered samples):

    |   ._.
    | ./   \.
    |/       \.
    |__________
    a b c d e f

## Options

SimpleGraph takes a hash of options as its third argument. Here's what you can customise:

  eg. __parameter:__ [default] description

 * __width:__ [600] width of rendered image
 * __height:__ [250] height of rendered image
 * __leftGutter:__ [30] space to reserve to the left of the graph. Allocates space for y-axis caption and labels
 * __bottomGutter:__ [20] space to reserve above the graph. Allocates space for x-axis
 * __topGutter:__ [20] space to reserve below the graph
 * __labelColor:__ [#000] text color for all labels
 * __labelFont:__ ["Arial"] font for all labels
 * __labelFontSize:__ ["9px"] font size for all labels
 * __gridBorderColor:__ ["#ccc"] background grid color, points will be plotted on the grid
 * __drawPoints:__ [true] whether or not to draw points on the graph
 * __pointColor:__ ["#000"] point color
 * __pointRadius:__ [3] point radius
 * __activePointRadius:__ [5] active point radius - used when hovering on points
 * __drawLine:__ [true] whether or not to join points on the graph with a line
 * __lineColor:__ ["#000"] self explanatory yah?
 * __lineWidth:__ [3] self explanatory yah?
 * __lineJoin:__ ["round"] round | miter | bevel - how to join the lines on the graph
 * __fillUnderLine:__ [false] fill under lines
 * __fillColor:__ ["#000"]
 * __fillOpacity:__ [0.2]
 * __drawBars:__ [false] want a bar graph?
 * __barColor:__ ["#000"] need I explain?
 * __addHover:__ [true] oh hover.. displays a little popup with y and x axis values for the selected point
 * __mysteryFactor:__ [0] it's a mystery

## Contributors

Dmitry Baranovskiy provided all of the initial code for plotting points on a graph using Raphael
Ben Askins took that example and created the SimpleGraph function
Lachie Cox improved sample code
Lachlan Hardy removed lint
Martin Stannard added bar graphs
Colin Campbell-McPherson eliminated repetition from setStyleDefaults

[Fork it on github](http://github.com/benaskins/simplegraph)

Send feedback & suggestions to ben.askins [at] gmail.com

## License

Copyright (c) 2008 Ben Askins

Licensed under the [MIT license](http://www.opensource.org/licenses/mit-license.php).

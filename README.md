d3po
====

Yet another Javascript library for making d3 charts. After playing with
[nvd3](http://nvd3.org) I found it wasn't quite as usable as I would like,
e.g. it wasn't very easy to add both points and lines to the same chart.
This library works as follows:

    var chart = d3po.chart();
    chart.lines([{x:0,y:3},{x:2,y:5}],{stroke:'blue'}])
    chart.points([{x:0,y:3.1,size:3,fill:'blue'},{x:0.5,y:2.5,size:5,fill:'red'}]);

I wanted a charting library that 'just works', like those you find in R or python.
Flexible where it needs to be, unobtrusive API that is amenable to embedding
in other settings (e.g. [IPython notebook](http://ipython.org/notebook.html)),
with helpful interactivity.

[Examples](http://adamlabadorf.github.io/src/d3po/src/test.html)


Dependencies
------------

[jQuery](http://jquery.com) and [d3](http://d3js.org).

Work in progress
----------------

Implemented:

    - scatter
    - lines
    - boxes (heatmap primitive, bar charts)
    - heatmap
    - axes
    - tooltips on hover over points
    - d3 zoom behavior (can be turned off)
    - html-based controls

Still lots of features to implement:

    - search feature
    - documentation (nvd3 is pretty bad about this as of this writing)

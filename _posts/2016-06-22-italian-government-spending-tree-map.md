---
layout: post
title: "A tree map of the Italian government spendings"
date: 2016-6-22
category: 
  - views
tag:
  - experiments
comments: true
show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
---

Using [D3plus](http://d3plus.org/) I try to give a figure on the **spendings** of the Italian Government.

<!--more-->

Tree map delle spese del governo italiano (dati del 2012, cifre in milardi di €)

## Spese del governo italiano (dati del 2012, [fonte](http://www.oggi.it/attualita/notizie/2012/06/11/stato-sprecone-i-ministeri-ci-costano-un-miliardo-di-euro-al-giorno/))

<script src="https://d3js.org/d3.v3.min.js"></script>

<script src="https://damianobacci.github.io/files/d3plus.js"></script>

<div id="viz"></div>

<script>
  var sample_data = [
    {"value": 100, "name": "Lavoro e politiche sociali"},
    {"value": 79, "name": "Economia e finanze"},
    {"value": 44, "name": "Istruzione e università"},
    {"value": 19, "name": "Difesa"},
    {"value": 11, "name": "Interno"},
    {"value": 7.6, "name": "Infrastrutture e trasporti"},
    {"value": 7.2, "name": "Sviluppo economico"},
    {"value": 7.2, "name": "Giustizia"},
    {"value": 1.7, "name": "Affari esteri"},
    {"value": 0.9, "name": "Salute"},
  ]

  var visualization = d3plus.viz()
    .container("#viz")  
    .data(sample_data)  
    .type("tree_map")   
    .id("name")         
    .size("value")      
    .draw()             
</script>

## Code

{% highlight js %}
<!-- load D3js -->
<script src="https://d3js.org/d3.v3.min.js"></script>

<!-- load D3plus after D3js -->
<script src="https://damianobacci.github.io/files/d3plus.js"></script>

<!-- create container element for visualization -->
<div id="viz"></div>

<script>
  // sample data array
  var sample_data = [
  {"value": 100, "name": "Lavoro e politiche sociali"},
    {"value": 79, "name": "Economia e finanze"},
    {"value": 44, "name": "Istruzione e università"},
    {"value": 19, "name": "Difesa"},
    {"value": 11, "name": "Interno"},
    {"value": 7.6, "name": "Infrastrutture e trasporti"},
    {"value": 7.2, "name": "Sviluppo economico"},
    {"value": 7.2, "name": "Giustizia"},
    {"value": 1.7, "name": "Affari esteri"},
    {"value": 0.9, "name": "Salute"},
  ]
  // instantiate d3plus
  var visualization = d3plus.viz()
    .container("#viz")  // container DIV to hold the visualization
    .data(sample_data)  // data to use with the visualization
    .type("tree_map")   // visualization type
    .id("name")         // key for which our data is unique on
    .size("value")      // sizing of blocks
    .draw()             // finally, draw the visualization!
</script>
{% endhighlight %}








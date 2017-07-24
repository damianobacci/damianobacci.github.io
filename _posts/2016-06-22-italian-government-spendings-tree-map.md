---
layout: post
title: "A tree map of the Italian government spendings"
date: "2016-6-22"
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

Tree map delle spese del governo italiano.

## Spese del governo italiano (dati del 2012, cifre in miliardi di €, [fonte](http://www.oggi.it/attualita/notizie/2012/06/11/stato-sprecone-i-ministeri-ci-costano-un-miliardo-di-euro-al-giorno/))

<script src="https://d3js.org/d3.v3.min.js"></script>

<script src="https://damianobacci.github.io/files/d3plus.js"></script>

<div id="viz"></div>

<script>
  var sample_data = [
    {"Spesa in miliardi": 100, "name": "Lavoro e politiche sociali"},
    {"Spesa in miliardi": 79, "name": "Economia e finanze"},
    {"Spesa in miliardi": 44, "name": "Istruzione e università"},
    {"Spesa in miliardi": 19, "name": "Difesa"},
    {"Spesa in miliardi": 11, "name": "Interno"},
    {"Spesa in miliardi": 7.6, "name": "Infrastrutture e trasporti"},
    {"Spesa in miliardi": 7.2, "name": "Sviluppo economico"},
    {"Spesa in miliardi": 7.2, "name": "Giustizia"},
    {"Spesa in miliardi": 1.7, "name": "Affari esteri"},
    {"Spesa in miliardi": 0.9, "name": "Salute"},
  ]

  var visualization = d3plus.viz()
    .container("#viz")  
    .data(sample_data)  
    .type("tree_map")   
    .id("name")         
    .size("Spesa in miliardi")     
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
    {"Spesa in miliardi": 100, "name": "Lavoro e politiche sociali"},
    {"Spesa in miliardi": 79, "name": "Economia e finanze"},
    {"Spesa in miliardi": 44, "name": "Istruzione e università"},
    {"Spesa in miliardi": 19, "name": "Difesa"},
    {"Spesa in miliardi": 11, "name": "Interno"},
    {"Spesa in miliardi": 7.6, "name": "Infrastrutture e trasporti"},
    {"Spesa in miliardi": 7.2, "name": "Sviluppo economico"},
    {"Spesa in miliardi": 7.2, "name": "Giustizia"},
    {"Spesa in miliardi": 1.7, "name": "Affari esteri"},
    {"Spesa in miliardi": 0.9, "name": "Salute"},
  ]
  // instantiate d3plus
  var visualization = d3plus.viz()
    .container("#viz")  // container DIV to hold the viz
    .data(sample_data)  // data to use with the viz
    .type("tree_map")   // visualization type
    .id("name")     // key for which our data is unique on
    .size("Spesa in miliardi")    // sizing of blocks
    .draw()             // draw the viz!
</script>
{% endhighlight %}

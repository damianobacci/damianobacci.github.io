---
layout: post
title: "Visualizing PopSpotsNYC with Leaflet.js"
date: 2017-7-31
description: "Because our Pop Culture is important"
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

PopSpotsNYC is a wonderful website by Bob Egan tracking all the original locations of iconic pieces of art (paintings, album covers, famous photos).

<!--more-->

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.1.0/dist/leaflet.css"
  integrity="sha512-wcw6ts8Anuw10Mzh9Ytw4pylW8+NAD4ch3lqm9lzAsTxg0GFeJgoAtxuCLREZSC5lUXdVyo/7yfsqFjQ4S+aKw=="
  crossorigin=""/>
<script src="https://unpkg.com/leaflet@1.1.0/dist/leaflet.js"
    integrity="sha512-mNqn2Wg7tSToJhvHcqfzLMU6J4mkOImSPTxVZAdo+lcPlk+GhZmYgACEe0x35K7YzW1zJ7XyJV/TT1MrdXvMcA=="
    crossorigin=""></script>
<div id="map" width="400px" height="400px"></div>
<script>
var	map	=	L.map('map',{center:	[35.10418,	-106.62987], zoom:	10 });
L.tileLayer('https://{s}.tile.osm.org/{z}/{x}/{y}.png').addTo(map);
</script>

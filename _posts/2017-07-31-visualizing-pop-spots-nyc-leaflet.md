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

<link rel="stylesheet" href="https://cdn.jsdelivr.net/leaflet/1.0.3/leaflet.css">
<script src="https://cdn.jsdelivr.net/leaflet/1.0.3/leaflet.js"></script>
<div	id="map"	style="width:	600px;	height:	400px"></div>
<script> var	map	=	L.map('map',	{ center:	[35.10418,	-106.62987], zoom:	10 });
L.tileLayer('https://{s}.tile.osm.org/{z}/{x}/{y}.png').addTo(map);
</script>

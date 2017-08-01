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

[PopSpotsNYC](http://www.popspotsnyc.com/) is a wonderful website by **Bob Egan** tracking all the **original locations** of iconic **pieces of art** (paintings, album covers, famous photos) in New York City.

<!--more-->

For this project I'm going to experiment a bit with [Leaflet.js](http://leafletjs.com), a powerful library to create beautiful and embeddable maps.

<link rel="stylesheet" href="https://cdn.jsdelivr.net/leaflet/1.0.3/leaflet.css">
<script src="https://cdn.jsdelivr.net/leaflet/1.0.3/leaflet.js"></script>
<style>
body {
    padding:	0;
    margin:	0;				
}
html,	body,	#map	{
    height:	100%;
    width: auto;								
}
</style>
<div	id="map"	style="width:	600px;	height:	400px"></div>
<script>
var	map	=	L.map('map',	{ center:	[40.7339,	-74.0245], zoom:	12 });
L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png').addTo(map);
var dylanIcon = L.icon({
        iconUrl: 'https://damianobacci.github.io/images/media/dylan-icon.png',
        iconSize: [38, 38],
        popupAnchor: [0,-15]
        });
var ramonesIcon = L.icon({
                iconUrl: 'https://damianobacci.github.io/images/media/ramones-icon.png',
                iconSize: [38, 38],
                popupAnchor: [0,-15]
                });
var bbIcon = L.icon({
                iconUrl: 'https://damianobacci.github.io/images/media/beastie-boys-logo.png',
                iconSize: [38, 38],
                popupAnchor: [0,-15]
                });
var vanIcon = L.icon({
                                iconUrl: 'https://damianobacci.github.io/images/media/van-morrison-icon.png',
                                iconSize: [38, 38],
                                popupAnchor: [0,-15]
                                });
var willieIcon = L.icon({
                                                iconUrl: 'https://damianobacci.github.io/images/media/willie-colon-icon.jpg',
                                                iconSize: [38, 38],
                                                popupAnchor: [0,-15]
                                                });
var breckerIcon = L.icon({iconUrl: 'https://damianobacci.github.io/images/media/brecker-icon.png', iconSize: [38, 38], popupAnchor: [0,-15]});
var generalMusicIcon = L.icon({iconUrl: 'https://damianobacci.github.io/images/media/general-music.png', iconSize: [38, 38], popupAnchor: [0,-15]});
var rightBrosIcon = L.icon({iconUrl: 'https://damianobacci.github.io/images/media/right-bros-icon.png', iconSize: [38, 38], popupAnchor: [0,-15]});
var youngIcon = L.icon({iconUrl: 'https://damianobacci.github.io/images/media/neil-young.png', iconSize: [38, 38], popupAnchor: [0,-15]});
var bruceIcon = L.icon({iconUrl: 'https://damianobacci.github.io/images/media/bruce-springsteen.jpg', iconSize: [38, 38], popupAnchor: [0,-15]});
var simonIcon = L.icon({iconUrl: 'https://damianobacci.github.io/images/media/paul-simon.png', iconSize: [38, 40], popupAnchor: [0,-15]});
var westIcon = L.icon({iconUrl: 'https://damianobacci.github.io/images/media/west-side.png', iconSize: [38, 40], popupAnchor: [0,-15]});
var marker = L.marker([40.73154, -74.01018], {icon: dylanIcon}).bindPopup("<h4>Bob Dylan - Blonde on Blonde</h4><img src='https://damianobacci.github.io/images/media/dylan-blonde.jpg'>").addTo(map);
var marker2 = L.marker([40.76860, -73.98149], {icon: dylanIcon}).bindPopup("<h4>Bob Dylan - Modern Times</h4><img src='https://damianobacci.github.io/images/media/dylan-modern.jpg'>").addTo(map);
var marker3 = L.marker([40.72514, -73.99061], {icon: ramonesIcon}).bindPopup("<h4>Ramones - Ramones</h4><img src='https://damianobacci.github.io/images/media/ramones-self.jpg'>").addTo(map);
var marker4 = L.marker([40.72005, -73.98858], {icon: bbIcon}).bindPopup("<h4>Beastie Boys - Paul's Boutique</h4><img src='https://damianobacci.github.io/images/media/beastie-pauls.jpg'>").addTo(map);
var marker5 = L.marker([40.70645, -74.00685], {icon: vanIcon}).bindPopup("<h4>Van Morrison - Too Long In Exile</h4><img src='https://damianobacci.github.io/images/media/van-morrison-exile.jpg'>").addTo(map);
var marker6 = L.marker([40.70993, -74.00390], {icon: dylanIcon}).bindPopup("<h4>Bob Dylan - I Want You</h4><img src='https://damianobacci.github.io/images/media/dylan-want.jpg'><p><a href='http://www.popspotsnyc.com/satevepost/'>Page on PopSpotsNYC</a></p>").addTo(map);
var marker7 = L.marker([40.70821, -73.99887], {icon: willieIcon}).bindPopup("<h4>Willie Colon - Cosa Nuestra</h4><img src='https://damianobacci.github.io/images/media/willie-cosa.jpg'>").addTo(map);
var marker8 = L.marker([40.71248, -74.00660], {icon: breckerIcon}).bindPopup("<h4>The Brecker Brothers - Straphangin'</h4><img src='https://damianobacci.github.io/images/media/brecker-strap.gif'>").addTo(map);
var marker8 = L.marker([40.70514, -74.00977], {icon: generalMusicIcon}).bindPopup("<h4>The Fifth Avenue Band - self-titled</h4><img src='https://damianobacci.github.io/images/media/fifth-avenue.jpg'>").addTo(map);
var marker9 = L.marker([40.70542, -74.01894], {icon: rightBrosIcon}).bindPopup("<h4>The Righteous Brothers - Go Ahed and Cry</h4><img src='https://damianobacci.github.io/images/media/right-bros-cry.jpg'>").addTo(map);
var marker10 = L.marker([40.73023, -73.99935], {icon: youngIcon}).bindPopup("<h4>Neil Young - After the Gold Rush</h4><img src='https://damianobacci.github.io/images/media/young-gold.jpg'><p><a href='http://www.popspotsnyc.com/afterthegoldrush'>Page on PopSpotsNYC</a></p>").addTo(map);
var marker11 = L.marker([40.73829, -73.98677], {icon: dylanIcon}).bindPopup("<h4>Bob Dylan - Highway 61 Revisited</h4><img src='https://damianobacci.github.io/images/media/dylan-highway.jpg'><p><a href='http://www.popspotsnyc.com/highway_61_revisited/index.html'>Page on PopSpotsNYC</a></p>").addTo(map);
var marker12 = L.marker([40.7628, -73.9839], {icon: dylanIcon}).bindPopup("<h4>Bob Dylan - Another Side of Bob Dylan</h4><img src='https://damianobacci.github.io/images/media/dylan-another.jpg'><p><a href='http://www.popspotsnyc.com/highway_61_revisited/index.html'>Page on PopSpotsNYC</a></p>").addTo(map);
var marker13 = L.marker([40.76640, -73.99032], {icon: bruceIcon}).bindPopup("<h4>Photo of Bruce Springsteen on Tenth Avenue</h4><img src='https://damianobacci.github.io/images/media/bruce-tenth.jpg'><p><a href='http://www.popspotsnyc.com/tenthavenue/'>Page on PopSpotsNYC</a></p>").addTo(map);
var marker14 = L.marker([40.71997, -74.00034], {icon: simonIcon}).bindPopup("<h4>Paul Simon - Still Crazy After All These Years</h4><img src='https://damianobacci.github.io/images/media/simon-crazy.jpg'><p><a href='http://www.popspotsnyc.com/stillcrazy/'>Page on PopSpotsNYC</a></p>").addTo(map);
var marker15 = L.marker([40.7390, -73.9900], {icon: dylanIcon}).bindPopup("<h4>Bob Dylan - Chronicles</h4><img src='https://damianobacci.github.io/images/media/dylan-chronicles.jpg'><p><a href='http://www.popspotsnyc.com/chronicles/'>Page on PopSpotsNYC</a></p>").addTo(map);
var marker16 = L.marker([40.76764, -73.98735], {icon: westIcon}).bindPopup("<h4>West Side Story - Original Broadway Cast Album</h4><img src='https://damianobacci.github.io/images/media/west-side-album.jpg'><p><a href='http://www.popspotsnyc.com/westsidestory/'>Page on PopSpotsNYC</a></p>").addTo(map);
</script>

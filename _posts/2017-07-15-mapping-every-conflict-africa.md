---
layout: post
title: Mapping every incident in Africa
date: "2017-7-15"
description: "Visualizing the troubled history of Africa"
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

The **ACLED** (Armed Conflict Location and Data Event Project) is a project directed by Professor [**Clionadh Raleigh**](http://www.sussex.ac.uk/profiles/320441) of the University of Sussex whose mission is to map every conflict event in Africa and South East Asia.

<!--more-->
<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/CGNZnVduOc4' frameborder='0' allowfullscreen></iframe></div>
(suggested listening)


This is a fantastic dataset that it's publicly available [here](http://www.acleddata.com/data/). You can feel that there is a huge number of stories about *struggle*, *death* and *conflicts* hidden between all those lines. It has been a big source for personal projects about Africa, and an invaluable piece of data that can help us understand what is going on through the entire continent.

I tried to visualize here all the conflicts based on the number of fatalities on [CARTO](https://carto.com).

There are many things that **I don't like** with this visualization, that mainly come from my poor understanding of the platform, or its limits (I can't really judge).

* the size of the circle should be proportional to the number of casualties
* there should be different colours for the different type of conflicts
* there should be a better way of selecting the actors involved
* I only used victims and perpetrators to filter the dataset, the [codebook](http://www.acleddata.com/wp-content/uploads/2017/01/ACLED_Codebook_2017.pdf) also lists *interaction codes* (Military VS Military, Rebels VS Rioters, Military VS Civilians etc..) that are very interesting to investigate

My plan is to build various stories that can use this dataset as a source (and a similar one of the [**Uppsala Conflict Data Program**](http://ucdp.uu.se/)).

<iframe width="100%" height="520" frameborder="0" src="https://damianobacci.carto.com/builder/9ea35fda-6d55-11e7-bcfc-0ef24382571b/embed" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

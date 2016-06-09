---
layout: post
title: Data Story n°2 - Rentswatch
# date element overrides date in title format.
date: 2016-6-8
description: "Data Story is a section of the website that provides an overview on a brilliant journalism project involving data. This time I talk about Rentswatch, an project done by the folks at Journalism++ tracking rent's price in Europe."
category:
  - views
tag:
  - data stories
comments: true
published: true
show_meta: true
comments: true
mathjax: true
gistembed: true
noindex: false
nofollow: false
---

*Data Story* is a section of the website that provides an overview on **a brilliant journalism project involving data**. This time I talk about [**Rentswatch**](http://www.rentswatch.com/), an project done by the folks at [**Journalism++**](http://www.jplusplus.org/en/) tracking rent's price in Europe.

<!--more-->

# Being young in Europe (and Italy [sigh])

I must say that I haven't any problems with rent prices because, at the age of **25**, I still live with my parents. **Are you surprised?** In Italy men tend to leave their home late in their 30s, as reported by [Eurostat]() (2013 data). Compared to other European countries we fair pretty poorly:


<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/_a7g69kXn_o' frameborder='0' allowfullscreen></iframe></div>

<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.8.2/jquery.min.js">
</script>
<script src="http://code.highcharts.com/highcharts.js">
</script>
<script src="http://code.highcharts.com/modules/exporting.js">
</script>

<div id="container" style="min-width: 310px; height: 400px; margin: 0 auto">
</div>

<script type="text/javascript">

$(function () {
        $('#container').highcharts({
            title: {
                text: 'Monthly Average Temperature',
                x: -20 //center
            },
            subtitle: {
                text: 'Source: WorldClimate.com',
                x: -20
            },
            xAxis: {
                categories: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
                    'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
            },
            yAxis: {
                title: {
                    text: 'Temperature (°C)'
                },
                plotLines: [{
                    value: 0,
                    width: 1,
                    color: '#808080'
                }]
            },
            tooltip: {
                valueSuffix: '°C'
            },
            legend: {
                layout: 'vertical',
                align: 'right',
                verticalAlign: 'middle',
                borderWidth: 0
            },
            series: [{
                name: 'Tokyo',
                data: [7.0, 6.9, 9.5, 14.5, 18.2, 21.5, 25.2, 26.5, 23.3, 18.3, 13.9, 9.6]
            }, {
                name: 'New York',
                data: [-0.2, 0.8, 5.7, 11.3, 17.0, 22.0, 24.8, 24.1, 20.1, 14.1, 8.6, 2.5]
            }, {
                name: 'Berlin',
                data: [-0.9, 0.6, 3.5, 8.4, 13.5, 17.0, 18.6, 17.9, 14.3, 9.0, 3.9, 1.0]
            }, {
                name: 'London',
                data: [3.9, 4.2, 5.7, 8.5, 11.9, 15.2, 17.0, 16.6, 14.2, 10.3, 6.6, 4.8]
            }]
        });
    });

</script>

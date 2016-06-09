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

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.8.2/jquery.min.js">
</script>
<script src="https://code.highcharts.com/highcharts.js">
</script>
<script src="https://code.highcharts.com/modules/exporting.js">
</script>

<div id="container" style="min-width: 310px; height: 400px; margin: 0 auto">
</div>

<script type="text/javascript">

        $('#container').highcharts({
            chart: {
            type: 'bar'
        },
        title: {
            text: 'Historic World Population by Region'
        },
        subtitle: {
            text: 'Source: <a href="https://en.wikipedia.org/wiki/World_population">Wikipedia.org</a>'
        },
        xAxis: {
            categories: ['Africa', 'America', 'Asia', 'Europe', 'Oceania'],
            title: {
                text: null
            }
        },
        yAxis: {
            min: 0,
            title: {
                text: 'Population (millions)',
                align: 'high'
            },
            labels: {
                overflow: 'justify'
            }
        },
        tooltip: {
            valueSuffix: ' millions'
        },
        plotOptions: {
            bar: {
                dataLabels: {
                    enabled: true
                }
            }
        },
        legend: {
            layout: 'vertical',
            align: 'right',
            verticalAlign: 'top',
            x: -40,
            y: 80,
            floating: true,
            borderWidth: 1,
            backgroundColor: ((Highcharts.theme && Highcharts.theme.legendBackgroundColor) || '#FFFFFF'),
            shadow: true
        },
        credits: {
            enabled: false
        },
        series: [{
            name: 'Year 1800',
            data: [107, 31, 635, 203, 2]
        }, {
            name: 'Year 1900',
            data: [133, 156, 947, 408, 6]
        }, {
            name: 'Year 2012',
            data: [1052, 954, 4250, 740, 38]
        }]
    });

</script>

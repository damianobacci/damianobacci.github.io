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

I must say that I haven't any problems with rent prices because, at the age of **25**, I still live with my parents. **Are you surprised?** In Italy men tend to leave their home late in their 30s, as reported by [Eurostat](http://ec.europa.eu/eurostat/product?code=yth_demo_030&language=en&mode=view). Compared to other European countries we fair pretty poorly:

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
            type: 'column'
        },
        title: {
            text: 'Estimated mean age of leaving the parental household, by sex, 2015'
        },
        subtitle: {
            text: 'Source: <a href="http://ec.europa.eu/eurostat/product?code=yth_demo_030&language=en&mode=view">Eurostat</a>'
        },
        xAxis: {
            categories: [
                'EU-28',
                'Croatia',
                'Italy',
                'Greece',
                'Spain',
                'Turkey',
                'Austria',
                'Belgium',
                'United Kingdom',
                'France',
                'Germany',
                'Netherlands',
                'Estonia',
                'Finland',
                'Denmark',
                'Sweden'
            ],
            crosshair: true
        },
        yAxis: {
            min: 0,
            title: {
                text: 'Years'
            }
        },
        tooltip: {
            headerFormat: '<span style="font-size:10px">{point.key}</span><table>',
            pointFormat: '<tr><td style="color:{series.color};padding:0">{series.name}: </td>' +
                '<td style="padding:0"><b>{point.y:.1f} mean age</b></td></tr>',
            footerFormat: '</table>',
            shared: true,
            useHTML: true
        },
        plotOptions: {
            column: {
                pointPadding: 0.2,
                borderWidth: 0
            }
        },
        series: [{
            name: 'Men',
            data: [27.2, 33.0, 31.3, 30.8, 30.1, 29.8, 26.6, 25.8, 25.3, 24.8, 24.6, 24.5, 24.1, 22.6, 21.5, 19.7]

        }, {
            name: 'Women',
            data: [25.1, 29.6, 29.0, 28.0, 28.0, 24.9, 24.3, 24.1, 23.6, 23.0, 22.9, 22.9, 23.1, 21.1, 20.8, 19.6]

        }]
    });

</script>


<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/_a7g69kXn_o' frameborder='0' allowfullscreen></iframe></div>
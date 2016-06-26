---
layout: post
title: Brexit Data
# date element overrides date in title format.
date: 2016-6-26
description: "Data Story is a section of the website that provides an overview on a brilliant journalism project involving data. This time I talk about Confiscati Bene, an italian project collecting datasets of assets seized from the mafia."
category:
  - views
tag:
  - experiments
comments: true
published: true
show_meta: true
comments: true
mathjax: true
gistembed: true
noindex: false
nofollow: false
---

Brexit data

<!--more-->

<script src="https://code.jquery.com/jquery-1.9.1.js"></script>

<script src="https://code.highcharts.com/highcharts.js">
</script>

<script src="https://code.highcharts.com/modules/exporting.js">
</script>

<div id="container" style="min-width: 310px; max-width: 800px; height: 400px; margin: 0 auto"></div>

<script type="text/javascript">

// Data gathered from http://populationpyramid.net/germany/2015/
    // Age categories

    var categories = ['West Midlands', 'East Midlands', 'North East', 'Yorkshire and The Humber',
            'East', 'North West', 'South West', 'Wales', 'South East',
            'Northern Ireland', 'London', 'Scotland'];

        $('#container').highcharts({
            chart: {
                type: 'bar'
            },
            title: {
                text: 'Vote breakdown across the UK'
            },
            subtitle: {
                text: 'Source: <a href="http://www.bbc.com/news/uk-politics-32810887">The UK Referendum, all you need to know</a>'
            },
            xAxis: [{
                categories: categories,
                reversed: false,
                labels: {
                    step: 1
                }
            }, { // mirror axis on right side
                opposite: true,
                reversed: false,
                categories: categories,
                linkedTo: 0,
                labels: {
                    step: 1
                }
            }],
            yAxis: {
                title: {
                    text: null
                },
                labels: {
                    formatter: function () {
                        return Math.abs(this.value) + '%';
                    }
                }
            },

            plotOptions: {
                series: {
                    stacking: 'normal'
                }
            },

            tooltip: {
                formatter: function () {
                    return '<b>' + this.series.name + ', age ' + this.point.category + '</b><br/>' +
                        'Population: ' + Highcharts.numberFormat(Math.abs(this.point.y), 0 + '%');
                }
            },

            series: [{
                name: 'Leave',
                data: [-59.3, -58.8, -58.0, -57.7, -56.5, -53.7, -52.6,
                    -52.5, -51.8, -44.2, -40.1, -38.0]
            }, {
                name: 'Remain',
                data: [40.7, 41.2, 42.0, 42.3, 43.5, 46.3, 47.4, 47.5,
                    48.2, 55.8, 59.9, 62.0]
            }]
        });

</script>


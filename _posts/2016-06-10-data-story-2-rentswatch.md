---
layout: post
title: Data Story n°2 - Rentswatch
# date element overrides date in title format.
date: "2016-6-10"
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

### Being young in Europe (and in Italy [sigh])

I must say that I haven't any problems with rent prices because, at the age of **25**, *I still live with my parents*. **Are you surprised?** In Italy men tend to leave their home late in their 30s, as reported by [Eurostat](http://ec.europa.eu/eurostat/product?code=yth_demo_030&language=en&mode=view). Compared to other European countries we fair pretty poorly:

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

This phenomenon is known in Italy as being a *"bamboccione"* (big baby), and it's related to a tons of factors, first of all the lack of stabile income and a poor job market.The fact that the italian welfare system is [**profoundly unbalanced**](https://www.bancaditalia.it/pubblicazioni/altri-atti-seminari/2013/paper-Ferrera.pdf) to older generations and some privileged professions of course doesn't help.

Being an underprivileged generation, rent prices are a big problem for younger people, especially in big cities. I can count many examples of friends in **Rome** struggling to find a decent apartment at a fair price, battling illegal contracts against lunatic landlords. While this is happening on a daily basis everywhere, [some premium apartments are rented for **ridiculously low** prices](https://www.theguardian.com/world/2016/feb/03/rome-reveals-apartments-with-historic-views-rented-out-for-a-few-euros-a-month) in the middle of the historic centre because they probably know the *right people* to talk to.

In the middle of this chaos, *how can we help as journalists?*

### Explaining Rentswatch

<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/_a7g69kXn_o' frameborder='0' allowfullscreen></iframe></div>

[**Rentswatch**](http://www.rentswatch.com/) is a database created by [**Journalism++**](http://www.jplusplus.org/en/), and it can show many informations about rent price in Europe's biggest cities.

#### The quiz

{:.text-center img}
![Rentswatch's quiz]({{ site.urlimg }}media/rentswatch-quiz.png "Rentswatch's quiz") [Rentswatch's quiz](http://www.rentswatch.com/#!/quiz/)

First of all, it'll let you take [**a quiz**](http://www.rentswatch.com/#!/quiz/) to determine if you pay *the right rent for the right flat*. It does so by analyzing your rent and flat's size, comparing them with the average of all the flats collected across Europe. The prices are scanned with a [*scraper*](http://blog.rentswatch.com/writing-scrapers/) coded with **Python**. But of course, prices can vary within different cities, so Rentswatch compare your price with the nearby apartments.

{:.text-center img}
![Rentswatch's result]({{ site.urlimg }}media/rentswatch-result.png "Rentswatch's result") Rentswatch's result

#### Map of rents in your city

{:.text-center img}
![Rentswatch's map]({{ site.urlimg }}media/rentswatch-map.png "Rentswatch's map") [Rentswatch's map](http://www.rentswatch.com/#!/city/)

Rentswatch can show [**a map**](http://www.rentswatch.com/#!/city/) of the various rents in a given city (not just *administrative boundaries*, but also **the metropolitan area**), comparing them between districts.

## The Mission - "Rentswatch aims at fostering quality journalism on the housing crisis"

[**Nicolas Kayser-Bril**](https://twitter.com/nicolaskb), cofounder and CEO of Journalism++, in [the opening blog's post](http://blog.rentswatch.com/all-the-rents-all-the-time/) is making a clear statement:

> Suprisingly, very little data exists regarding the price of rents. Cities do run studies on the topic. Countries do, too. But such data is rarely compatible (a rent in Berlin does not encompass the same elements as a rent in Bucharest). No single Europe-wide database is available for someone who ponders moving out of a city.

> We want to change that. We will provide a database of rents, all across Europe, all the time, for free. We will use all possible sources of information to achieve this. This will not solve the issue of unaffordable housing, but it will give a little more information - and power - to renters when they sign a contract.

The database is *continuously growing in number*, and the data is available to media partners via the [**Rentwatch's API**](http://blog.rentswatch.com/api/). Overall, with the Rentswatch project we can see a **perfect example** of how we can use the technology to *collect and organize precious informations*, which otherwise could be **lost** in the sea of messy data that unfolds during our daily life. It's time for journalists *to harness to power of technology* to analyze this complex world better (and **faster**) than before. This project in *on the right track to do so*.

You can find other examples in [the blog](http://blog.rentswatch.com/), and you can follow [**@rentswatch**](https://twitter.com/rentswatch) on Twitter for updates.

<a class="twitter-timeline" data-width="500" data-height="500" data-dnt="true" href="https://twitter.com/rentswatch">Tweets by rentswatch</a> <script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

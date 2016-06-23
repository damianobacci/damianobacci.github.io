---
layout: post
title: "A tree map of the Unseen64 archive"
date: 2016-6-23
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

Using [Highcharts](http://www.highcharts.com/) I picture all the games in the [Unseen64](https://www.unseen64.net) archive (it's the best website ever, consider supporting us on [Patreon](https://www.patreon.com/unseen64?ty=h)).

<!--more-->

## Unseen64 Games Archive (per console data)

<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/1.8.2/jquery.min.js"></script>
        
<script type="text/javascript">

$(function () {
    $('#container').highcharts({
        series: [{
            type: "treemap",
            layoutAlgorithm: 'stripes',
            alternateStartingDirection: true,
            levels: [{
                level: 1,
                layoutAlgorithm: 'sliceAndDice',
                dataLabels: {
                    enabled: true,
                    align: 'left',
                    verticalAlign: 'top',
                    style: {
                        fontSize: '15px',
                        fontWeight: 'bold'
                    }
                }
            }],
            data: [{
                id: 'A',
                name: 'Apples',
                color: "#EC2500"
            }, {
                id: 'B',
                name: 'Bananas',
                color: "#ECE100"
            }, {
                id: 'O',
                name: 'Oranges',
                color: '#EC9800'
            }, {
                name: 'Anne',
                parent: 'A',
                value: 5
            }, {
                name: 'Rick',
                parent: 'A',
                value: 3
            }, {
                name: 'Peter',
                parent: 'A',
                value: 4
            }, {
                name: 'Anne',
                parent: 'B',
                value: 4
            }, {
                name: 'Rick',
                parent: 'B',
                value: 10
            }, {
                name: 'Peter',
                parent: 'B',
                value: 1
            }, {
                name: 'Anne',
                parent: 'O',
                value: 1
            }, {
                name: 'Rick',
                parent: 'O',
                value: 3
            }, {
                name: 'Peter',
                parent: 'O',
                value: 3
            }, {
                name: 'Susanne',
                parent: 'Kiwi',
                value: 2,
                color: '#9EDE00'
            }]
        }],
        title: {
            text: 'Fruit consumption'
        }
    });
});

</script>

<script src="https://code.highcharts.com/highcharts.js"></script>

<script src="https://code.highcharts.com/modules/treemap.js"></script>

<div id="container"></div>

## Code

{% highlight js %}

{% endhighlight %}








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

<script src="https://code.jquery.com/jquery-1.9.1.js"></script>

<script src="https://code.highcharts.com/highcharts.js"></script>

<script src="https://code.highcharts.com/modules/treemap.js"></script>

<div id="container" style="min-width: 300px; max-width: 600px; margin: 0 auto">
</div>
        
<script type="text/javascript">

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
                id: 'MS',
                name: 'Microsoft',
                color: "#107c10"
            }, {
                id: 'N',
                name: 'Nintendo',
                color: "#D20014"
            }, {
                id: 'S',
                name: 'Sony',
                color: '#000000'
            }, {
                id: 'SG',
                name: 'Sega',
                color: '#17569b'
            }, {
                id: 'O',
                name: 'Others',
                color: '#BECCD1'
            }, {
                name: 'Xbox',
                parent: 'MS',
                value: 307
            }, {
                name: 'Xbox One',
                parent: 'MS',
                value: 296
            }, {
                name: 'DS',
                parent: 'N',
                value: 78
            }, {
                name: 'Game Boy',
                parent: 'N',
                value: 53
            }, {
                name: 'Game Boy Advance',
                parent: 'N',
                value: 94
            }, {
                name: 'GameCube',
                parent: 'N',
                value: 142
            }, {
                name: 'NES/Famicom',
                parent: 'N',
                value: 101
            }, {
                name: 'Nintendo 3DS',
                parent: 'N',
                value: 9
            }, {
                name: 'Nintendo 64 & 64DD',
                parent: 'N',
                value: 158
            }, {
                name: 'SNES',
                parent: 'N',
                value: 144
            }, {
                name: 'Virtual Boy',
                parent: 'N',
                value: 11
            }, {
                name: 'Wii',
                parent: 'N',
                value: 101
            }, {
                name: 'WiiU',
                parent: 'N',
                value: 3
            }, {
                name: 'Others',
                parent: 'O',
                value: 480
            }, {
                name: '32X / Mega CD',
                parent: 'SG',
                value: 45
            }, {
                name: 'Dreamcast',
                parent: 'SG',
                value: 91
            }, {
                name: 'Game Gear',
                parent: 'SG',
                value: 13
            }, {
                name: 'Master System',
                parent: 'SG',
                value: 9
            }, {
                name: 'Mega Drive / Genesis',
                parent: 'SG',
                value: 92
            }, {
                name: 'Saturn',
                parent: 'SG',
                value: 87
            }, {
                name: 'Playstation',
                parent: 'S',
                value: 242
            }, {
                name: 'Playstation 2 (PS2)',
                parent: 'S',
                value: 372
            }, {
                name: 'Playstation 3 (PS3)',
                parent: 'S',
                value: 239
            }, {
                name: 'PSP',
                parent: 'S',
                value: 48
            }, {
                name: 'PS Vita',
                parent: 'S',
                value: 1
            }]
        }],
        title: {
            text: 'Unseen64 Games Archive'
        }
    });

</script>

## Code

{% highlight js %}

<script src="https://code.jquery.com/jquery-1.9.1.js"></script>

<script src="https://code.highcharts.com/highcharts.js"></script>

<script src="https://code.highcharts.com/modules/treemap.js"></script>

<div id="container" style="min-width: 300px; max-width: 600px; margin: 0 auto">
</div>
        
<script type="text/javascript">

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
                id: 'MS',
                name: 'Microsoft',
                color: "#107c10"
            }, {
                id: 'N',
                name: 'Nintendo',
                color: "#D20014"
            }, {
                id: 'S',
                name: 'Sony',
                color: '#000000'
            }, {
                id: 'SG',
                name: 'Sega',
                color: '#17569b'
            }, {
                id: 'O',
                name: 'Others',
                color: '#BECCD1'
            }, {
                name: 'Xbox',
                parent: 'MS',
                value: 307
            }, {
                name: 'Xbox One',
                parent: 'MS',
                value: 296
            }, {
                name: 'DS',
                parent: 'N',
                value: 78
            }, {
                name: 'Game Boy',
                parent: 'N',
                value: 53
            }, {
                name: 'Game Boy Advance',
                parent: 'N',
                value: 94
            }, {
                name: 'GameCube',
                parent: 'N',
                value: 142
            }, {
                name: 'NES/Famicom',
                parent: 'N',
                value: 101
            }, {
                name: 'Nintendo 3DS',
                parent: 'N',
                value: 9
            }, {
                name: 'Nintendo 64 & 64DD',
                parent: 'N',
                value: 158
            }, {
                name: 'SNES',
                parent: 'N',
                value: 144
            }, {
                name: 'Virtual Boy',
                parent: 'N',
                value: 11
            }, {
                name: 'Wii',
                parent: 'N',
                value: 101
            }, {
                name: 'WiiU',
                parent: 'N',
                value: 3
            }, {
                name: 'Others',
                parent: 'O',
                value: 480
            }, {
                name: '32X / Mega CD',
                parent: 'SG',
                value: 45
            }, {
                name: 'Dreamcast',
                parent: 'SG',
                value: 91
            }, {
                name: 'Game Gear',
                parent: 'SG',
                value: 13
            }, {
                name: 'Master System',
                parent: 'SG',
                value: 9
            }, {
                name: 'Mega Drive / Genesis',
                parent: 'SG',
                value: 92
            }, {
                name: 'Saturn',
                parent: 'SG',
                value: 87
            }, {
                name: 'Playstation',
                parent: 'S',
                value: 242
            }, {
                name: 'Playstation 2 (PS2)',
                parent: 'S',
                value: 372
            }, {
                name: 'Playstation 3 (PS3)',
                parent: 'S',
                value: 239
            }, {
                name: 'PSP',
                parent: 'S',
                value: 48
            }, {
                name: 'PS Vita',
                parent: 'S',
                value: 1
            }]
        }],
        title: {
            text: 'Unseen64 Games Archive'
        }
    });

{% endhighlight %}








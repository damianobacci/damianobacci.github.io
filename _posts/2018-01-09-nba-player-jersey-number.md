---
layout: post
title: "How many NBA players have the same jersey number and why?"
date: 2018-1-09
description: "Basketball!"
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
Basketball and data journalism have come a long way together. If you missed the stuff that [**Kirk Goldsberry**](https://twitter.com/kirkgoldsberry) was doing on [Grantland](https://grantland.com/contributors/kirk-goldsberry/) (RIP) or all the magic that is now possible with [SportVU](https://www.youtube.com/watch?v=jOQEl_tkEwE) and [cameras](https://news.usc.edu/70358/you-call-the-shots-on-the-video-board-thanks-to-usc-computer-scientists/) then you have a lot to catch up.

<!--more-->

I decided to do a quick experiment after a talk with ex-teammates about **jersey numbers**. Back in the day some of us picked a number depending on their relation with a star player (number 8 and 24 for **Kobe**, number 23 for **Jordan**, 15 for **Vince Carter** etc) or for other futile motives (69...). I tried to check if I could find *some patterns* in jersey numbers that has been used in the NBA up until now.

I used a database available online on [Basketball-Reference.com](https://www.basketball-reference.com/friv/numbers.cgi), a great source for NBA statistics and other cool stuff basketball-related.

This dataset has been scraped using the [Scraper Chrome browser extension](https://chrome.google.com/webstore/detail/scraper/mbigbapnjcgaffohmbkdlecaccepngjd) and hosted on Google Drive.

<iframe width="405px" height="500px" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSsg0IaOY9n15wPfwUD-61WSxcv4nbzhcnJ6wrrBrAvv5CD7hUL47qihrXgAq3E2Avhkt8jmGYViDx2/pubhtml?widget=true&amp;headers=false"></iframe>
<br>
The data visualization has been done with [RAWGraphs](http://rawgraphs.io/), an Italian data visualization platform based on D3.js.

<a href="https://damianobacci.github.io/images/media/nba-numbers.svg" target="_blank">
<img src="https://damianobacci.github.io/images/media/nba-numbers.svg">
</a> (click to enlarge)
<br>
### Finding patterns

We can find some interesting patterns by simply look up at the data: for example we can clearly see that there is a sharp drop for numbers **16-19**, **26-29**, **36-39**, **46-49**, completely disappearing after 55.

The reason is pretty simple and it has nothing to do with the NBA itself, but with the rule regarding jersey numbers in high school and NCAA college. The NBA is now an international league but up until the 80s not many foreign players were allowed, thus the near total of the players came from NCAA colleges, which have a particular rule regarding jersey number:

{:.text-center img}
![NCAA allowed numbers]({{ site.urlimg }}media/ncaa-rule-numbers.png "NCAA allowed numbers")

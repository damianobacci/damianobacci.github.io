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

The reason is pretty simple and it has nothing to do with the NBA itself, but with the rule regarding jersey numbers in **high school** and **NCAA college**. The NBA is now an international league but up until the 80s not many foreign players were allowed, thus the near total of the players came from NCAA colleges, which have a **particular rule** regarding jersey numbers ([from NCAA Rule 1, Section 22, Article 7, clause b.2](https://ncaambb.arbitersports.com/Groups/104883/Library/files/BR15.pdf)):

{:.text-center img}
![NCAA allowed numbers]({{ site.urlimg }}media/ncaa-rule-numbers.png "NCAA allowed numbers")

Since players *tend to retain the same number they wore in college*, we can pretty much understand this difference in the data.
This rule has been applied at least since the 60s, because famous college players of the lates 50s like **Bill Russell** could wore different numbers (Russell wore n.6 at the University of San Francisco).

[Zach Schonbrun](https://twitter.com/zschonbrun) wrote a [piece on the New York Times](https://www.nytimes.com/2015/03/31/sports/ncaabasketball/numerals-on-college-basketball-jerseys-you-can-count-them-on-one-hand.html) citing the lack of numbers in some colleges, based on the fact that many numbers has been retired during these years.

There are some nice quotes explaining the origin of this strange rule (which is not used in Europe, albeit there were different limitations):

> The uniform policy — adhered to by the N.C.A.A. and the National Federation of State High School Associations (the national governing body for high school athletics) — is said to be intended to simplify the hand signaling made by officials.
When a player is whistled for a foul, the referee signals to the scorer’s table the uniform number of the offender by using his hands. John Adams, the N.C.A.A.’s men’s basketball officiating coordinator, said the system is set up so that referees flash only two hands to make their signals, making things easier for the scorer to interpret.

You can see a video of the **flashing signal** in action here (of course it seems pretty stupid because the rest of the world is following the FIBA rules for signaling numbers, which use both hands).

<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/8lgTxzgvmzw' frameborder='0' allowfullscreen></iframe></div>

### Fun side note

In the chart there are also number **0** and **00**, which are not uncommon (but they can't exist at the same time on the same team). However at the end you can notice numbers like **03**, **07** and **09**.

Those numbers belong the the [**Rochester Royals**](https://en.wikipedia.org/wiki/1950%E2%80%9351_Rochester_Royals_season), one of the incarnations of the present-day **Sacramento Kings**:

* **03** has been used by [**Pep Saul**]() during the 1949-50 and 1950-51 seasons, by [**Sam Ranzino**]() through the 1951-52 season and by [**Jack McMahon**]() from 1953 to 1955.
* **07** has been used by [**Paul Noel**]() through the 1950-51 season.
* **09** has been used by [**Bobby Wanzer**]() during all his tenure with the Rochester Royals, from 1949 to 1955 (Wanzer was a Hall of Famer and the first NBA player to shoot over 90 percent from the free-throw line in a season)

I still can't explain why only the Royals had these numbers, maybe there is a funny story somewhere waiting to be told.

{:.text-center img}
![Rochester Royals 1951-52]({{ site.urlimg }}media/rochester-royals-1951.jpg "Rochester Royals 1951-52")

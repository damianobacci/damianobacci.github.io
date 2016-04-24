---
layout: post
title: Data Journalism at IJF16
# date element overrides date in title format.
date: 2016-4-16
tag:
  - tutorial
  - scraping
  - python
  - excel
  - cleaning
  - visualization
  - qgis
comments: true
show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
---

The [International Journalism Festival](http://www.journalismfestival.com) (**IJF**) is a journalism festival held in [Perugia](https://en.wikipedia.org/wiki/Perugia) every year, with a moltitude of panel discussions, workshops and presentations done by over [500 speakers](http://www.journalismfestival.com/speaker-list/2016). In the 2016 edition I had the chance to volunteer at the festival, and so I was able to attend many sessions devoted to [data journalism topics](http://www.journalismfestival.com/programme/2016/category/data-journalism-school) Here's a list of what I found interesting.

<!--more-->

First of all, I have to tell you that you can view all past events of IJF **for free** on [**its Youtube channel**](https://www.youtube.com/channel/UClUtH75j6Bd7_Ty17jHVDPg). Unfortunately there is **no translation available**, this means that even if there was a translation during the event you can only listen to the original audio. I hope they'll fix this problem in the future.

This year the festival was packed with data journalism events, I think it was the first time in which I was obliged to choose between two simultaneous panels that interested me. A lot of them were done by the amazing [**Dataninja**](http://www.dataninja.it/), an independent team of journalists and tech people focusing on **data journalism**, **visualizations**, **open data** and **geo data**. I had the opportunity to meet them and I can assure you about their passion and their knowledge. Other amazing workshops were done by [**Marco Túlio Pires**](https://twitter.com/mtrpires), manager of the [**School of Data**](http://schoolofdata.org/). Not only they were very **interesting and useful**, but Marco has an **amazing knack for teaching**, I hope you will check them out.

Let's dive in!

## [Tools for the collection, organization and analysis of data](http://www.journalismfestival.com/programme/2016/tools-for-the-collection-organization-and-analysis-of-data) ([slides available](http://slides.com/dataninja/tool-raccolta-analisi-dati#/))
<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/VRkImNi_O1g' frameborder='0' allowfullscreen></iframe></div>
**Who**: [Andrea Nelson Mauro](https://twitter.com/nelsonmau), [Gianluca De Martino](https://twitter.com/glucademartino)

**What**: Andrea opens the panel with a brief introduction about Dataninja and their past works, including the elearning platform [**Dataninja School**](http://school.dataninja.it/). Gianluca then talks about different scraping tools like [**Tabula**](http://tabula.technology/) and [**ScraperWiki**](https://scraperwiki.com/), and Andrea demonstrates how to use the [**Scraper** extension](https://chrome.google.com/webstore/detail/scraper/mbigbapnjcgaffohmbkdlecaccepngjd) for Google Chrome. The resulting spreadsheet is then put on [**Google Spreadsheets**](http://sheets.google.com), filtered and analyzed using a [**pivot table**](https://en.wikipedia.org/wiki/Pivot_table). They proceed to talk about [**OpenRefine**](http://openrefine.org/) and how it can be used to clean your data.

## [Joining multiple Excel files with Python](http://www.journalismfestival.com/programme/2016/joining-multiple-excel-files-with-python-hands-on) ([slides available](https://goo.gl/Kl0RKs))

<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/t5MBwcOsSF4' frameborder='0' allowfullscreen></iframe></div>
**Who**: [Marco Túlio Pires](https://twitter.com/mtrpires)

**What**: This session focus on using [**Python**](https://www.python.org/) to work with your spreadsheets data, an additional tutorial is available on [the relevant repository](https://github.com/mtrpires/pyPerugia16) on [Marco's GitHub page](https://github.com/mtrpires). A little knowledge of Python and [**regular expressions**](https://en.wikipedia.org/wiki/Regular_expression) is required, make sure to check [this course](https://www.edx.org/course/introduction-computer-science-mitx-6-00-1x-7) on **edX** about computer science and Python.

## [Free data journalism tools](http://www.journalismfestival.com/programme/2016/free-data-journalism-tools) ([slides available](https://goo.gl/bdILgh))

<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/_HYiV_skkek' frameborder='0' allowfullscreen></iframe></div>
**Who**: [Marco Túlio Pires](https://twitter.com/mtrpires)

**What**: Half an hour of amazing **free tools** for everything data journalism related.

### Get the data

* `importHTML` function in Google spreadsheets
* [**WebScraper extension**](https://chrome.google.com/webstore/detail/web-scraper/jnhgnonknehpejjnehehllkliplmbmhn) for Google Chrome
* [**If This Then That**](https://ifttt.com/): an amazing website that connects a whole bunch of services on the Internet. As soon as something that you set up happens or triggers, it does something else (like collecting all Instagram pictures in a determined location)

### Clean the data 

* The evergreen [**OpenRefine**](http://openrefine.org/)
* [Google Spreadsheets' **formulas**](https://support.google.com/docs/table/25273?hl=en), like `=split()`,`=trim()`,`=proper()` and `=clean`
* [**DataWrangler**](http://vis.stanford.edu/wrangler/) from Stanford University

### Analyze the data

* **Pivot Tables** in Google Spreadsheets
* [**Python Pandas**](http://pandas.pydata.org/), huge tool using Python for statistical analysis (make sure to check [this book](http://shop.oreilly.com/product/0636920023784.do) for further infos)
* [**GNU PSPP**](https://www.gnu.org/software/pspp/) for statistical analysis of big datasets, based on [IBM's SPSS](https://en.wikipedia.org/wiki/SPSS)

### Visualize data

* [**Chartbuilder**](https://quartz.github.io/Chartbuilder/) for simple data visualization
* [**RAW**](http://raw.densitydesign.org/): the missing link between spreadsheets and vector graphics, for more complex visualization
* [**CartoDB**](https://cartodb.com/) for maps

### Tell the story

* [**Atavist**](https://atavist.com/), a powerful tool for media-rich stories
* [**Timeline.js**](https://timeline.knightlab.com/) for interactive timelines
* [**Silk.co**](https://www.silk.co/) for interactive data visualization

## [Fancy becoming a GEOrnalist?](http://www.journalismfestival.com/programme/2016/fancy-becoming-a-geornalist)

<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/g8etYruJrmA' frameborder='0' allowfullscreen></iframe></div>
**Who**: [Andrea Borruso](https://twitter.com/aborruso)

**What**: Andrea introduces [**QGIS**](http://qgis.org/) and various problems related to map and coordinates. He then demonstrates how it can be used to create beautiful maps, using geodata found in public datasets and data scraped from Twitter. Recommended lectures: [QGIS Map Design](http://www.amazon.com/QGIS-Map-Design-Anita-Graser/dp/0989421759/ref=pd_sim_14_3/179-1268518-5643253?ie=UTF8&dpID=51gUMD6e2-L&dpSrc=sims&preST=_AC_UL160_SR131%2C160_&refRID=1SJB7JK72KCM7N5YVNBX) and [Learning QGIS Second Edition](http://www.amazon.com/Learning-QGIS-Second-Anita-Graser/dp/1784392030) by **Anita Graser**.

## [Tips and tricks for data-driven journalism starters](http://www.journalismfestival.com/programme/2016/tips-and-tricks-for-data-driven-journalism-starters)

<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/yvrsK_vtDLk' frameborder='0' allowfullscreen></iframe></div>
**Who**: [Bahareh Heravi](https://twitter.com/Bahareh360)

**What**: 
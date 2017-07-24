---
layout: post
title: Data Story n°1 - Confiscati Bene
# date element overrides date in title format.
date: "2016-6-2"
description: "Data Story is a section of the website that provides an overview on a brilliant journalism project involving data. This time I talk about Confiscati Bene, an italian project collecting datasets of assets seized from the mafia."
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

*Data Story* is a section of the website that provides an overview on **a brilliant journalism project involving data**. This time I talk about [**Confiscati Bene**](http://www.confiscatibene.it/), an italian project collecting datasets of assets seized from the mafia.

<!--more-->

### "Mafia Corporation"

[**Organized crimes**](https://en.wikipedia.org/wiki/Organized_crime_in_Italy) is still a big problem in Italy. Recently, the italian police seized [something like **500 million €**](http://www.globaltimes.cn/content/975192.shtml) (563 million $) in a raid against the Iannazzo crime family of the [**'Ndrangheta**](https://en.wikipedia.org/wiki/%27Ndrangheta), the most powerful crime syndicate in the country.

> The seized assets included 53 plots of real estate and farmland, 24 commercial buildings, 27 vehicles and shares of at least 21 companies, the organized crime investigation group of Italy's finance police said in a statement. [...]
One of the region's largest shopping centers was among the properties taken by the Italian authorities.


Basically, [organized crime makes a ton of money every year](http://www.theguardian.com/world/2014/mar/26/ndrangheta-mafia-mcdonalds-deutsche-bank-study). A report by [The Organised Crime Portfolio](http://www.ocportfolio.eu/) (OCP) estimates that the annual revenue for illicit markets in Italy may be as high as **29.480 millions €** (that includes *drugs, human and firearm trafficking*, *counterfeiting*, *extortion racketeering* and frauds*).

However, sometimes the authorities manage to block few of these illegal activities and confiscate the related goods. You can see a breakdown of confiscated goods in the table below:

<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='//embed.chartblocks.com/1.0/?c=574b3cf69973d2bf5287fa3f&t=c6b560cbf013b25' frameBorder='0'></iframe></div>

*But where does this stuff go?*

### Italy and confiscated goods

Despite the **importance of seized assets** for the fight against crime organization ([as remarked by the EU](http://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32014L0042)), the OCP's report underlines **several limitations** of the actual state of things:

> * Data are often collected within the same country by several
agencies, involved in different stages of the asset recovery
process or based in different geographic locations. This
means that statistics are not often available in a centralized
dataset, with uniform information;
* Data can refer to different stages of the asset recovery
process and even provide overlapping information on the
same court proceedings;
* It is often not possible to clearly distinguish the main
offence(s) for which an asset was confiscated;
* Other useful information (e.g. location and condition of
the confiscated asset, date of seizure/confiscation, type or
name of the related criminal group) is often missing;
* In most cases, assets are not associated with a unique
ID code throughout the recovery process, and this makes
it impossible tracing the assets throughout the whole
process.

These limitations still apply to Italy, even if in a smaller part. Italy has got **four databases about confiscated goods**:

* **SIPPI (SIT-MP) Database**, managed by the *Ministry of Justice*
* **SAC Database**, managed by the *Criminal Analysis Service – Servizio Analisi Criminale* (**SAC**) of the *Ministry of the Interior*
* **ANBSC Database**, managed by the **ANBSC** – *Agenzia Nazionale per l'amministrazione e la destinazione dei beni sequestrati e confiscati alla criminalità organizzata*, of the *Minister of the Interior*
* **Guardia di Finanza Database**

Wow, that's plenty of data! It's a shame that some of the databases *don't provide an easy access to it*. The first two don't provide publicly disaggregated information per each individual asset, while the Guardia di Finanza's one **is not even publicly available**! The ANBSC's one has got information at disaggregate level for each asset, but navigation is hard and confused. Last, neither of these informations is published in an **open format**.

### Confiscati Bene ("Well Confiscated")

{:.text-center img}
![Map of Italy's confiscated goods]({{ site.urlimg }}media/confiscati-bene-map.png "Map of Italy's confiscated goods") Map of Italy's confiscated goods

A group of italian journalists and civic activists decided to **help on this matter**: during the annual meeting on open data called [Spaghetti Open Data](http://www.spaghettiopendata.org/) they began to [scrape](http://damianobacci.github.io/tags/#scraping) the data from the ANBSC's website and publish it in *disaggregated format*, *refining and enriching* it with meta-informations (like geo-references) during the process. The resulting dataset was made public available on a [specific platform](http://www.confiscatibene.it/it/dataset), coupled with [choropleth maps](https://en.wikipedia.org/wiki/Choropleth_map).

The intention of the civic activist's group is clear: **open data** on something so important as confiscated goods is crucial, because **transparency and availability** of these sort of informations can help the society in a variety of ways, from relocating the assets (often they find a way to NGOs and other social organizations) to sending a potent signal of disturbance to criminal activities. Also, **journalists** can take advantages of this dataset, to help searching and curating stories, fostering a collective storytelling.

The website also has a vibrant community, where everyone can help others reporting confiscated goods missing, monitor them or request other data from the public administration.

You can find all the wonderful work of **Confiscati Bene** on [their website](http://www.confiscatibene.it/it), and follow them on Twitter at [@confiscatibene](https://twitter.com/confiscatibene)

<a class="twitter-timeline" href="https://twitter.com/confiscatibene" data-widget-id="737046188306878465">Tweet di @confiscatibene</a>
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");</script>

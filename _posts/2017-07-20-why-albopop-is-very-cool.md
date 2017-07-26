---
layout: post
title: "Why AlboPop is very very cool"
date: 2017-7-20
description: "AlboPop is a way of making 'more popular' the official council board of Italian public administrations, often buried behind old and closed web services."
category:
  - views
tag:
  - thoughts
comments: true
show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
---

[**AlboPop**](http://albopop.it/) is a small experiment created by [**Andrea Borruso**](https://twitter.com/aborruso) and [**OpenDataSicilia**](http://opendatasicilia.it/), a group of **passionate professionals** whose mission is improving public community's awareness and quality of life through [**Open Data**](https://en.wikipedia.org/wiki/Open_data) and [**Open Government**](https://en.wikipedia.org/wiki/Open_government).

<!--more-->

**AlboPop** is a way of making ‘more popular’ the **official council board** (also knows as *albo pretorio*) of Italian public administrations, often buried behind **old and closed web services**, by **integrating its feed into social networks**.

{:.text-center img}
![AlboPop]({{ site.urlimg }}media/albo-pop.png "AlboPop")

### What is an *Albo Pretorio*?

In the Italian administrative system, an *albo pretorio* is a space where **public administrations** are obliged by law to publish all sorts of **news and notices of public interest** for the community.

The *Comune* is the Italian word for [**municipality**](https://en.wikipedia.org/wiki/Municipality), a single urban administrative division having **corporate status** and powers of **self-government or jurisdiction**, and in Italy it represents the smallest administrative power. All *Comuni* are required to have an *albo pretorio* where they can publish their notices. These notices can be **decrees, order, regulations, call for council meetings** and many different public announcements concerning the local community.

You can think of the *albo pretorio* as a **public council noticeboard**, and I think that a comparable example (albeit more limited) with the UK reality could be the [modern.gov app](https://play.google.com/store/apps/details?id=uk.co.moderngov.modgov&feature=search_result#?t=W251bGwsMSwyLDEsInVrLmNvLm1vZGVybmdvdi5tb2Rnb3YiXQ)

The *albo pretorio* is an **important way** for the citizen to be **aware** and **engaged** about all the choices and process of the public administration: it's a precise stream of informations and data that it's **vital** for citizens. Unfortunately it's not so easy to have a proper access to these informations, and this is **harming our power to be informed** and **made correct decisions**.

### Albo Pretorio Online

All municipalities are required to have a link to the *albo pretorio* right on their homepage:

{:.text-center img}
![Albo Pretorio of Narni]({{ site.urlimg }}media/albo-pretorio-narni.png "Albo Pretorio of Narni") [Albo Pretorio of Narni](http://www.comune.terni.it/albo-pretorio)

**Problems** arise when you try to get **updates** on all the notices that are getting published every day (four or five per day): in the majority of *albi pretori* there is **no way in doing that**. That's because there is **no standard** for the platform of an online *albo pretorio*, so every municipality can potentially get a different system to manage it. Since every system works in a different way you can find yourself dealing with multiple way of **organizing data, filtering and sorting it,** etc...

For example, here are others *albi pretori* from Narni's nearby *Comuni*:

{:.text-center img}
![Albo Pretorio of Terni]({{ site.urlimg }}media/albo-pretorio-terni.png "Albo Pretorio of Terni") [Albo Pretorio of Terni](http://www.comune.terni.it/albo-pretorio)

{:.text-center img}
![Albo Pretorio of Amelia]({{ site.urlimg }}media/albo-pretorio-amelia.png "Albo Pretorio of Amelia") [Albo Pretorio of Amelia](http://albopretorio.datamanagement.it/?ente=comunediamelia&tipoSubmit=ricerca)

{:.text-center img}
![Albo Pretorio of Spoleto]({{ site.urlimg }}media/albo-pretorio-spoleto.png "Albo Pretorio of Spoleto") [Albo Pretorio of Spoleto](http://www.comunespoleto.gov.it/nuovo-albo-pretorio/)

{:.text-center img}
![Albo Pretorio of Orvieto]({{ site.urlimg }}media/albo-pretorio-orvieto.png "Albo Pretorio of Orvieto") [Albo Pretorio of Orvieto](http://albopretorio.webred.it/albo-c001/home.html)

As you can see, pretty much every *Comune* has a **different method** of managing its *albo pretorio*. Worst than that, there is **no way to get updates** when there is a new publication. Imagine being a citizen that wants to **monitor public choices, contracts** and so on: you are obliged to go to the website **every day** just to check if there are updates, and if you are not 100% committed you will probably lose interest during time.

**AlboPop** is a way to overcome this situation. It will make "**popular**" the *albo pretorio* by **integrating its feed in the social networks** that you utilizes the most.

### How AlboPop is done

There are **multiple ways** to make an Albopop, but the key concept is always the same:

* We have to build an `automatic scraper which goes to the webpage`{:.yelhglt} of an albo pretorio and `fetches particular informations that will be exported to a Google Sheet`{:.yelhglt}, a script will then `convert it to an RSS feed that can be published on Facebook, Twitter and Telegram`{:.yelhglt} using services like [**IFTTT**](https://ifttt.com/discover) or [**Zapier**](https://zapier.com/).

#### Known Problems

Of course there can be issues, especiallu when you are talking about **public administrations** and **computers**:

* All the notices could be behind a system using **cookies** to validate the session
* Infos can only be get through an **AJAX request**
* The scraper could stop to work if the **structure of the webpage is suddenly changed**

### AlboPop of Narni

Let's take a look on an easy example: the [AlboPop of Narni](http://albopop.it/comune/narni/).

The *Albo Pretorio* of Narni's municipality is hosted on a **common management platform** for municipality in Italy called [**Halleyweb**](http://www.halley.it/home/include/mostra_foto_allegato.php?servizio_egov=sa&idtesto=63&&nodo=nodo26), and this makes easier to scrape information on the page.

The basic part of the operations is having the `IMPORTXML` function on a Google Sheet to scrape content, and using **XPATH queries** to direct the scraping to the elements that we want (these will be the **description** of the notice, what **type** of notice is, the **publication and end date** and eventually a **link** to attachments)

XPATH queries are located in a subsheet called *meta*, which contains other informations (author, specs, geolocation):

{:.text-center img}
![Google Sheet of an Albopop]({{ site.urlimg }}media/albopop-sheet.png "Google Sheet of an Albopop")

All the informations are located in the subsheet *raccolta* (collection), and then they are refined and filtered in another subsheet called *clean*, so we can have exact and ordered infos:

{:.text-center img}
![Google Sheet of an Albopop]({{ site.urlimg }}media/albopop-sheet2.png "Google Sheet of an Albopop")

Now it's time to **transform this text into a RSS feed**, and this process is done with a script created by [**Matteo Fortini**](https://twitter.com/matt_fortini):

{:.text-center img}
![2RSS script]({{ site.urlimg }}media/albopop-2rss.png "2RSS script")

When the script is deployed it generates our **RSS Feed** that we can then export to a service like [**FeedBurner**](https://feedburner.google.com):

{:.text-center img}
![Feedburner page of Narni's Albopop]({{ site.urlimg }}media/albopop-feedburner.png "Feedburner page of Narni's Albopop")

Then it's pretty easy to set up an integration with a **Facebook page**:

{:.text-center img}
![Facebook page of Narni's Albopop]({{ site.urlimg }}media/albopop-fb.jpg "Facebook page of Narni's Albopop")

A **Twitter account**:

{:.text-center img}
![Twitter account of Narni's Albopop]({{ site.urlimg }}media/albopop-tw.jpg "Facebook page of Narni's Albopop")

Or a **Telegram channel** (using a **Telegram bot**):

{:.text-center img}
![Telegram channel of Narni's Albopop]({{ site.urlimg }}media/albopop-telegram.jpg "Telegram channel of Narni's Albopop")

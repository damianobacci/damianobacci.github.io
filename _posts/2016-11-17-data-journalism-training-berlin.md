---
layout: post
title: Data Journalism Training Camp in Berlin "Prejudice against migration"
# date element overrides date in title format.
date: 2016-11-17
category:
  - views
tag:
  - tutorial
  - thoughts
comments: true
published: true
show_meta: true
comments: true
mathjax: true
gistembed: true
noindex: false
nofollow: false
---

# Data-driven journalism against prejudices about migration

@(Data Journalism Training)

*Berlin, 12 – 20 November 2016*

<!--more-->

**People**
*Nika* - Media production
*Anastasia* - Schedule related
*Martin* - administration
*Sergei* - technical program?
*Marzia* - migration

#### What is Data Journalism?

=/ *journalism with data*
Data = when is a **source** for your story
- Jon Snow and chloera disease in London
- Florence Nightingale and soldier's health care
- Afghan War logs for Wikileaks (*Alastair Dent and David Leigh*)
- Migrants' Files
- Medical response time lags in LA (*LA Times*)
- **Crowdsourcing**: GPS recording of cycling

**Legal and source material for data?**

#### Data pipeline

Find -> Get -> Verify -> Clean -> Analyse -> Present

```flow
st=>start: Find
e=>end: Present
op=>operation: Get
op2=>operation: Verify
op3=>operation: Clean
op5=>operation: ANalyse
op6=>operation: Present

st->op->op2->op3->op4
```

**Find the Data**
- Using search engine (**Google**, **Bing**, **Yahoo** & advanced operation)
- NGOs
- Network of contacts/sources/website

**Get the data**
- Scraping PDF & web pages (*Python**)
- Accessing machine readble files

**Verify**
*do not trust your dataset*
- Origins
- Meta data
- Every method has limitation (check methodology)

**Cleaning data**
- Errors
- Open Refine

**Analyse Data**
- Extract meaningful information

**Present data**
- Visualization

### Talks about different field of expertise

**Martin Rentsch** . *UNHCR*
What is behind refugee protection?
- Countries must protect citizens
- BUT they persecute them
- THAT'S WHY they flee to another country
- Without the Geneva's Convention this country is not obliged to deal with these people

***GENEVA'S REFUGEE CONVENTION***
- Who's a refugee (feels of being persecuted for reasons of *race*, *religion*, *nationality*, *mermbership of a particular social group or political opinion*) **Refugee** or **Migrant** (*IOM*)?
- Legal protection
- Assistance and social rights
- Obligations
- Exclusion clauses
- 65.3 millions persons of concerns (21.3 Refugees, 5.2 Pakistan refugees, 40.8 internally displaced people [IDPs], 3.2 asylum seekers)
- [Photos and video](media.unhcr.org)
- [Data](data.unhcr.org) -> [*Global Trends on Migration*](popstats.unhcr.org)
- [Operations](reporting.unhcr.org)
-
**Ola Aljari** - Overview of Media Mistakes and biases when reporting refugee
> Jounalists often fail to tell the full story and routinely fallinto propaganda traps laid by politicians

**Ethical Journalism Report**
- Missed Opportunities (did not raise the alarm about the influx of refugeees coming from Syria and Iraq before 2015)
- Hate speech (by politicians)
> outrageous anti-migrant or anti-Muslin like Donald Trump

- Fallling Standards (no specialize refugee journalists, nobody goes really deep into the problem). Some journalists admittted thei inability to cover some stories
- Sensationalism (media outlets failed to follow good media standards and instead used wrong term to describe refugees)

***Solutions***
- Specialized reporters on migrations
- Focus on training and issues (good media outlets are interested)
- Improved link with migrants (report on all sides of concerns and fears. Migrants have also their concerns, understand both sides and introduce to each others)
- Journalist from ethnic minority communities (language skills, cultural and social background)
- We also need to put aside the political agendas forced by parties and politicians and dig deep for the "real reasons" of the crisis
- Focus on the long term results, instead focusing on the current challenges

**Marzia Bona** [Osservatorio Balcani e Caucaso](http://www.balcanicaucaso.org/)
- Balkan Route
- *"72h legislation"*
- "Hungarian **Wall**"
- Ill-equipped media systems (political elites and media system were confronted for the first time with such phenomenon **from outside**)
- Peculiarities of media systems (tabloidization [clickbaiting], lack of independence, media ownership concentration impact on pluralism) ->difference in terms (clandestini/migranti)

**Nicolas Kayser-Bril**
- [Bit.ly presentation](bit.ly/tmf-wannsee)
 > "Measuring what should be measure"

*Grants by JournalismFund.eu*

Problem:
- The Money Trails
- Counting the Dead

1) Some data existed (*Fortress Europe*, *Gabriele del Grande*, *Puls* by University of Helsinki) [Not comprehensive]
2) Reports were many times plain texts

Geolocalize with CARTO, Visualize (water or land?)

#### **Daria** from project work
- **0** data of sexual violence in the world
- different type to categorize sexual violence
- **What do you count as data?**

#### Data solution for migration issues - Yuliana (Der Spiegel)
- About 1.8 million IDP in Ukraine
- Show tendency and scales
- Cloud highcharts, QGis, Illustrator
 [link for inspiration and work](spiegel.de/thema/daten)

#### Sources of data - Martin (UNHCR)

- Statistics and **Global Trends Report** (tables.xls)
- popstats.unhcr.org - definitions, legal terms, how do we count them. Create your own query (*persons of concern*) / Asylum seekers section / Resettlement
- data.unhcr.org - most recent data / Most pressing crisis / Migrants Emergency Response
- reporting. unhcr.org

#### Others source of data - Marzia

- Eurostat (statistics explained, level of metadata)
- Eurobarometer (public opinion survey)
- Eurodac statistics
- European Asylum Support Office (**EASO**)
- European Union Open Data Portal (Open data on EU institution and their functioning)
- European Data Portal (National statistics from all EU countries)
- European Migration Network (it aims to provide updated, objective reliable & comparable information on migration and asylum)
- European Council on Refugees and Exiles (**ECRE**)
- **FRONTEX** (European Border and Coast Guard Agency)
- Open Migration
- GlobalStat
- Local NGOs

#### **Gianna Gruen** - *Extracting data. get it in useful format and organize your data*

- Always search for the **answer** not the question
- Use **Google Advanced Search** for finding data (filetype:pdf option and different languages) or *different search engines*
- **Right to be forgotten**
- Google **Alerts**, **Changedetection.com** and **Talkwalker**
- **Update Scanner** for Firefox
- Google Shortcuts (see webguide)

#### Scraping data from PDF
- Use **splitpdf.com** to access to a page
- Use **cometdocs** to scrape the page and download the table (or **Zamzar**, **Tabula**, **Pdftoexcel**)
- **Documents Clouds** or **Lime OCR** to process your Image-based PDF
#### Scraping data from PNG
- Upload your image to **Google Docs** and open it in Google Docs
####Scraping from Website
- Chrome extension **Scraper**

#### Suggestions to organize
- Name the files with an useful name
- Always work in a copy of the original
- Track the changes you make
#####Checklist
- Are you working in a copy of the original?
- Do you have all the data you need, organized in worksheets?
- Are the cells in the format they should be?
- Do you have any formatting issues? ()thousand-separators can cause trouble, sometimes figures are converted to dates, are all letters represented correctly or might you have an encoding problem)

#### Excels commands
`-SUM()`, `-AVERAGE()`, `-COUNT()`
- Percentage change
- Copy formulae
- Apply filter
- Relative and absolute references  `$A$1 vs A1`
- **Filter data** `AND`,`OR`, `IF` functions

**AND**
Returns TRUE/FALSE if ALL expressions are true
Syntax: =AND(logical_expression1, [logical_expression2, ...])

**OR**
Returns TRUE/FALSE if ANY of the expressions is true
Syntax: =OR(logical_expression1, [logical_expression2, ...])  

**IF**
Returns customized phrases for passing and failing the logical test
Syntax: =IF(logical_expression, value_if_true, value_if_false)

#### VLOOKUP

(see guide)

#### Make yourself a database

Become a data expert of your city/region/country

- General data
- Specific data

**Don't store anything**
**DATA IS NOT NEUTRAL** - Why is an agency collecting this data? Why is collected/what for? What might be biases? *Data not necessarily describe reality*

### SCRAPING

A lot of application are driven with API

##### WHY DO I NEED TO SCRAPE?
Data isn't always in the format we wants

[Python the Hard Way](https://learnpythonthehardway.org/)

``` python
thing_1 = 1
thing_2 = 2

print (thing_1 + thing_2)

import request # request information from website
url = "http://www.parliament.co.uk/"
thePage = request.get(url) # .get -> method inside a library that helps out

print(thePage)
 - virtualenv env # how to run different version of Python
 source ./env # to make sure that it's active

# import HTML from a website

from ixml import html
url = "http://www.parliament.co.uk/"
thePage = request.get(url) # .get -> method inside a library that helps out

tree = html.fromstring(thePage.content)
theDead = tree.xpath('//*[@id="top"]/div[5]/div[1]/div/div/p[1]'

print(theDead) # take a specific part of the table

# BeautifulSoup, navigating around blocks of HTML

import BeautifulSoup

def MakeSoup

page = requests.get(url)
soupdata = BeautifulSoup(page.content)

table = soup.find(id="deceasedLords")
print(table)
```

You can use two different version of a library with **ENV**

*Python* can help you understand different type of programming languages, because it gives you the general basics of programming
You can use Python to understand how *Javascript* works.

- Be "respectful" when you are running a script, because it may cause conflicts with APIs
- Slack: News .... (ask)
- Mailing list (ask)
- **Hacks/Hackers** (Milan)
- [**Chaos Computers Club**](https://events.ccc.de/congress/)

### Open Refine by Nicolas Kayser-Bril

Right between spreadsheets and databases, you see **rows** and **columns**, but like a database *cells are not linked* with each other.

What is good at?
- Clean messy data
- Browse data by facet ()
- Connect data to the web of APIs

What is not good at?
- Input data
- Pivot tables

Your tables has to make *sub sense*, we don't know if it's one person or one incident

**Facet**: unique values in the column we decided to facet
**Undo**:  list of passages of your operations
*It's reproducibile!*, you can trace your steps - **Transparency, usability, you can load your previous list of steps** (*very useful*)

What are the logical steps to create a new column with the value female with all the females

### Data Analysis(OKI DE - Open Knowledge Germany) - Anna Alberts & Michael Peters
#### Basic Statistics

- The science of organizing, analysing, representing and collecting data

##### Descriptive statistics
- Measure of central tendency (on *average*)
- Measure of spread (how are my data points *divided*?)

###### Central Tendency

- **Mean**, the average (all data points divided by the number of datapoints)
- **Median**, the value in the middle (all the values, for which we use N - and then half of N - that is your middle value) [look at income data, a billionaire can screw up the average]
- **Mode**, the most frequent value (the datapoint that appears the most, very important with *qualitative data*, or *rankings*)

###### Measure of spread
- **Range**, minimum to maximum
- **Variance**, the average of the *squared difference* from the Mean, how many data points are closed to the Mean? (how high things are changing?)

$$	{(mean - x)^2} $$

-  ** Standard deviation**, measure what is "normal" what is in the dataset [look for outliers] or expected (root square of the variance) -

The whole room is the **population**, the people picked are the **sample**
###### Normal Distribution

"Bell curve", **Central limit theorem** -> averages of random variables converge to the normal distribution if the number of observations is high enough (IQ Scores, test scores)

###### Correlation

**Mutual relation** of two or more things (ex. *Average Income per Age*) - ***linear regression*** (minimum distance from the line of the points)

- two variables x and y
- Y = dependent variable (to be explained) [shoe size]
- X = independent (explaining Y) [lenght of foot]
- **Correlation Cohefficient** (from -1 to +1, zero means zero correlation, 0.3+/- only after that you can call for a correlation) [Guess the Correlation](http://guessthecorrelation.com)
##### Inferences from data
> Correlation does not imply causation

Control variables -> *Use your common sense!*

- Is there a clear causal effect?
- Can you control other factors?
- Does the relationship hold up against reasonable doubt?

#### Storytelling with data (Gianna Gruber) [slides!!]

##### Data -> Story
- Data tells the story (more awareness of a pitfall: just because you wrote a story, it doesn't mean people are goind to read it)
- You get an impression for what can and cannot be conveyed with data
- *"Just a set of numbers!"*
##### Story -> Data
- Data is a part of the story
- More rich in context
- More natural for journalists
- Data for the sake of data?
##### Communicate data visually
***Text & Numbers VS Visuals*** (balance on how little and how much you want to show) What trends you see? Why do they compare?
##### When not to narrate with data visuals
- When you have only one number
- When your dataset is too small
- Not consistent data source (institution gather data differently
- If you can't phrase yout findings in a headline that you'd click, maybe there's no story to tell)
##### Challenge commonplaces/prejudices
- **Fact checking and testing hypothesis**
- **Comparing values**: contextualizing or constrasting data
- **In-depth interviews**: adding perspectives, check with the entity producing the data (talk to a UNHCR statiscian about your findings), talk with experts for possible explanations, confront politicians with your findings, talk with the people behind your numbers
- **Geo-distribution patterns**, identifying outliers (be aware of matching patterns)
- **Time-event analysis**, finding patterns
- **Network analysis**, showing invisible connections

##### 4 ideas to public a story
- What is the publications' beat?
- Who and where is your audience? Is it on mobile or desktop?
- Providing detail vs giving an overview?
- Does it need to be interactive?
- What is relevant for your narrative? What is not? *Don't drown in data!*

#### How to turn your idea into first draft

- Check what others have done already
- Help yourself having an overview and not get lost (write down your hypothesis in possible headlines, think about what data you need ti test those headlines, brainstorm 8 quetion you are asking your data)
- **Pitch your idea to colleagues**
- Keep track in a *data diary*
- Test first story draft with colleagues

#### Use this draft to create a structure
- Which information do you need to understand the story at any given point
- See `data visual` as medium like text, videos, photos

##### Portrait: challenge
- Enstablishing a protagonist
- Challenge is he up against
- possible solution
- outlook for protagonist
##### Feature: part of a trend
##### News: example
##### Background fact checks

### Data Visualization

**Loic**

##### Designing the data
**Processing** (software) - *Ben Fry*, new volume of data produced. In **France** data visualization is helping refugees -> [welcomemap.fr](http://welcomemap.fr), [Carte des camps de refugies](http://), [Les Monde's Decodeur](http://)
##### Artistic inspiration
**Johannes Ittem**, **Josef Albers**, **Otto Neurath**, **Edward Tufte** (*The visual display of quantitative information*) - keep most as data and don't fall in the illustrator side, data should always be more (*The cognitive style of Powerpoint*), **Manuel Lima** (*Visual Complexity*)
##### Good sense helper
- Don't scale your quantity, no small and big humans!
- Don't mess *Radius* vs *Surface* when comparing circles, use the surface because it's more precise
#### File formats
- **Static**: JPEG, GIF, PNG, PDF
- SVG in the middle
- **Interactive**: HTML, JAVASCRIPT, CSS
#### Different tools
- [**Adobe's Color**](http://color.adobe.com), it produces good contrast colors and good armony
- [**RegeXr**](http://www.regexr.com), test pattern in *GREL*
- **Infogr.am**, you should not use this if you want to have some long term use
- [**Google Charts**](http://developers.google.com/chart/)
- [**TimelineJS**](), **AEONTimeline**
- [**D3.js**](https://d3js.org/)
- [**LeafletJS**](), [marker cluster plug in](https://github.com/Leaflet/Leaflet.markercluster),  polyline plugin, mix d3 and Leaflet
- [**GeoJSon.io**]
- [**Mapbox**], GeoJSON, Chlorophlet
- [**Tableau**]
- [**Papa Parse**], tool to parse CSV files online

####Category, Time, Hierarchy, Location
All the different type of dataviz

####
There are some limitations to use some standard file in Javascript

#### Leaflet code example

``` javascript
<script type="text/javascript">


		var osmUrl		= 'http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'; // specify Open Street Map tile to Leaflet
		var osmAttrib	= 'Map data © <a href="http://openstreetmap.org">OpenStreetMap</a> contributors'; // attribution for copyright data
		var osmTiles	= new L.TileLayer(osmUrl, { // declaration of the tiles
			minZoom: 10,
			maxZoom: 18,
			attribution: osmAttrib // level of zoom on the tiles
		});


		var SouthWest 	 	= L.latLng(52.354659, 13.028051), // limitation of the declaration (coordinates)
		    NorthEast 	 	= L.latLng(52.707861, 13.696250), // you can find the coordinates on Google Maps
		    LimitsOfTheMap 	= L.latLngBounds(SouthWest, NorthEast);

		var map = new L.map('map',{
			// maxBounds: LimitsOfTheMap, // disable the ability to scroll outside of the bounds // of course remove the slash
			layers: [osmTiles]
		});

        map.fitBounds(LimitsOfTheMap); // fit the bounds defined, you fill the map with the coordinates given in this box

        // OR map.setView([51.505, -0.09], 13); or you say the central point and the level of zoom


	</script>
```
If you want to modify CSS properties of Open Street Map you can use a NodeJS library

#### Adding a GeoJSON file

``` javascript
<script type="text/javascript">


		var osmUrl		= 'http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png';
		var osmAttrib	= 'Map data © <a href="http://openstreetmap.org">OpenStreetMap</a> contributors';
		var osmTiles	= new L.TileLayer(osmUrl, {
			// minZoom: 10,
			// maxZoom: 18,
			attribution: osmAttrib
		});


		var SouthWest 	 	= L.latLng(52.354659, 13.028051),
		    NorthEast 	 	= L.latLng(52.707861, 13.696250),
		    LimitsOfTheMap 	= L.latLngBounds(SouthWest, NorthEast);

		var map = new L.map('map',{
			// maxBounds: LimitsOfTheMap, // enable or disable the ability to scroll outside of the bounds
			layers: [osmTiles]
		});
        map.fitBounds(LimitsOfTheMap); // fit the bounds defined

        // OR map.setView([51.505, -0.09], 13);

        // this is scanning the geojson file
		L.geoJSON(refugee_data, {
		    style: function(feature) {},
		    onEachFeature: forEachPointFinded //this is the call to a function for each point, to do something

		}).addTo(map);

		// this is the declaration of the function forEachPointFinded
		function forEachPointFinded(feature, layer) {
			// if a description is found
			if (feature.properties.description) {
				// we add a popup on the click event
				// the content of the popup is the Name and the description
		        layer.bindPopup("<h1>"+feature.properties.Name+"</h1><div>"+feature.properties.description+"</div>");
		    }
		}


	</script>
```
Example **JSON**
``` json
var refugee_data=[
"_comment":"added this before line to specify the GeoJSON file in Leaflet, because you have to refer your dataset, also the type: Feature needs to explained for GeoJSON type file"
    {
        "type": "Feature",
        "properties": {
            "Name": "Flugdach Nickelsdorf",
            "description": "<img src=\"https://pbs.twimg.com/media/CQhCEWXWEAEPfB1.jpg:large\" height=\"200\" width=\"auto\" /><br><br>Updated at: 17/10 22:00 CET<br>Nr. of refugees: no refugees<br>Situation: Following the borders' closure tonight by Hungary, some trains have passed through this border.
```
#### Pivot Tables and Tableau (Anastasia)

- Always make a copy of your sheet

FILTER: only data of different categories (only agriculture or others)
REMEMBER you have to sketch you table and think what data goes in the rows and in the columns

Measures: amount of money
Dimension: names


#### Mauro Espresso

Contenuti verticali, orizzontali, contenuti indipendenti che raccontino più storie, la storia dell'articolo più quella dei grafici (complementari) (max500px/550px), storytelling

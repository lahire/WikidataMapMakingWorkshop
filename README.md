# Map making workshop – from Wikidata to interactive off-Wiki maps in three steps

<image src="images/generic-workshop-opening.jpg" width="500"/><br clear="all"/>

## Workhop description 
In this 90-120 minutes workshop you will learn how to make both flat, layered, embedded and interactive maps from sets of geo-referenced ([P625](https://www.wikidata.org/wiki/Property:P625)) items in Wikidata. 

You will do this in 3 modules of approx. 30-40 minutes each:

* **Module 1**: We will start by making various basic flat maps in Wikidata using SPARQL queries. (Libraries example). Next we will make some layered maps, where groups of items can be toggled on/off in the map. (Libraries example)
* **Module 2**: After having explored maps in the Wikidata query interface, we are now ready to learn how we can embed Wikidata-driven maps in other Wikimedia projects, such as Wikipedia and Commons (see the example on the right). In addition to SPARQL we will look at GeoJson, OpenStreetMap and the Kartographer extentsion.
* **Module 3**: Finally, and if times allows, we will have a look at the steps for creating fully interactive Wikidata-driven maps that can be used off-Wiki, ie. in regular HTML pages. In addtition to the above tools & techniques, we will use some basic Python, Jupyter Notebooks (PAWS), Jupyter-Leaflet and Jupyter-widgets.

## Learning objectives
After the workshop you will
* Understand the steps to make basic flat and layered maps in Wikidata, based on geo-referenced (P625) items and SPARQL queries (Module 1, basic) 
* Understand steps to embed maps in Wikimedia sites like Wikipedia, Wikimedia Commons, Wikidata (Module 2, intermediate)
* Understand the steps to create Wikidata-based maps than can be used in other (non-Wiki) websites (Module 3, advanced)
* Have access to map making resources, SPARQL examples and Python code snippets they can build upon for their own projects.

## Intended audiences
While this workshop is tech-focused and will discuss basic Wikidata, Wikipedia and Wikimedia Commons techniques and programming tools, it is meant to be approachable by beginning Wikidata contributors and programmers. The workshop leader, by no means an advanced Python programmer nor Wikidata nor SPARQL guru himself, will be showing and sharing examples and code snippets that you can easily adapt yourself with basic SPARQL, Wikidata and Python skills, to make them work for your own datasets.

As the workshop is comprised of three 30-40 minute modules, you can decide to skip the modules that you find too advanced (or basic) for your individual knowledge level.

### Required preparations
In order to maximize the effective workshop time, you are requested to do some preparations before coming to the workshop:

* Identify a geo-referenced (P625) set of coherent items in Wikidata to work with. Aim for 100-500 items or so. ([some examples](OutlineAndNotes.md#module-1--basic-flat--layered-maps))
* Create an account on Wikidata/ Wikimedia, if not yet done so.
* Set up a working PAWS server and notebook ([Help 1](https://www.mediawiki.org/wiki/Manual:Pywikibot/PAWS), [Help 2](https://wikitech.wikimedia.org/wiki/PAWS), [Help 3](https://www.mediawiki.org/wiki/PAWS)) – only needed if you plan to follow Module 3

## Workshop outline & resources
A full outline of the workshop is available on  [this page](OutlineAndNotes.md)
## Resources 
### For entire workshop
* Full workshop outline and notes: [OutlineAndNotes.md](OutlineAndNotes.md) 
* Full workshop slides on [Slidehare]() and [Wikimedia Commons]()

### For Module 2
* https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019/

### For Module 3
* https://paws-public.wmflabs.org/paws-public/User:OlafJanssen/MapMakingWorkshop_Wikimania2019.ipynb (with [backup in this repo]( 	MapMakingWorkshop_Wikimania2019.ipynb))
* [Raw json version of this notebook](https://paws-public.wmflabs.org/paws-public/User:OlafJanssen/MapMakingWorkshop_Wikimania2019.ipynb?format=raw)

## Workshop leader and contact details
* This workshop is given by Olaf Janssen, Wikimedia coordinator of the national library of The Netherlands - https://www.kb.nl/wikipedia
* olaf.janssen@kb.nl
* User:OlafJanssen on (Dutch) Wikipedia, Wikimedia Commons and Wikidata
* Twitter: @ookgezellig

## Dates
so far, this workshop was given during
* [Wikimania 2019](https://wikimania.wikimedia.org/wiki/2019:Libraries/Map_making_workshop_%E2%80%93_from_Wikidata_to_interactive_off-wiki_maps_in_three_steps), Stockholm, 18-8-2019
* [WikidataCon](), Berlin, October 2019
* [Wiki Techstorm III](), Amsterdam, 22-11-2019
* [National library of The Netherlands](), The Hague, tbd








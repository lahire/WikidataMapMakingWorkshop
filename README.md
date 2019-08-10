# Map making workshop – from Wikidata to interactive off-Wiki maps in three steps

Original description of this workshop: https://wikimania.wikimedia.org/wiki/2019:Libraries/Map_making_workshop_%E2%80%93_from_Wikidata_to_interactive_off-wiki_maps_in_three_steps
([Archived URL](https://web.archive.org/web/20190808101032/https://wikimania.wikimedia.org/wiki/2019:Libraries/Map_making_workshop_%E2%80%93_from_Wikidata_to_interactive_off-wiki_maps_in_three_steps))

## Learning objectives
Participants will
* Understand the steps to make basic flat and layered maps in Wikidata, based on geo-referenced (P625) items and SPARQL queries (Module 1, basic) 
* Understand steps to embed maps in Wikimedia sites like Wikipedia, Wikimedia Commons, Wikidata (Module 2, intermediate)
* Understand the steps to create Wikidata-based maps than can be used in other (non-Wiki) websites (Module 3, advanced)
* Have access to map making resources, SPARQL examples and Python code snippets they can build upon for their own projects.

## Resources 

### For entire workshop
* Full workshop outline and notes: [OutlineAndNotes.md](OutlineAndNotes.md) 
* Full workshop slides on [Slidehare]() and [Wikimedia Commons]()

### For Module 2
* https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019/

### For Module 3
* https://paws-public.wmflabs.org/paws-public/User:OlafJanssen/MapMakingWorkshop_Wikimania2019.ipynb (with [backup in this repo]( 	MapMakingWorkshop_Wikimania2019.ipynb))
* [Raw json version of this notebook](https://paws-public.wmflabs.org/paws-public/User:OlafJanssen/MapMakingWorkshop_Wikimania2019.ipynb?format=raw)

## Contact details
* Olaf Janssen, national library of The Netherlands - https://www.kb.nl/wikipedia
* olaf.janssen@kb.nl
* User:OlafJanssen on (Dutch) Wikipedia, Wikimedia Commons and Wikidata
* Twitter: @ookgezellig

## Dates
This workshop was given during
* [Wikimania 2019](https://wikimania.wikimedia.org/wiki/2019:Libraries/Map_making_workshop_%E2%80%93_from_Wikidata_to_interactive_off-wiki_maps_in_three_steps), Stockholm, 18-8-2019
* [WikidataCon](), Berlin, October 2019
* [Wiki Techstorm III](), Amsterdam, 22-11-2019
* [National library of The Netherlands](), The Hague, tbd


Description

In this workshop you will learn how to make both flat, layered, embedded and interactive maps from sets of geo-referenced (P625) items in Wikidata. For instance mapping public libraries in The Netherlands

We will do this in 3 modules of approx. 30 minutes each:
+
-
30 km
Wikimedia Commons: DutchPublicLibrariesNorthHolland.map, Wikimedia maps | Map data © OpenStreetMap contributors
Map of public libraries in the province of North-Holland, The Netherlands. Work in progress, 7-6-2019

    Module 1: We will start by making various basic flat maps in Wikidata using SPARQL queries. (Libraries example). Next we will make some layered maps, where groups of items can be toggled on/off in the map. (Libraries example)
    Module 2: After having explored maps in the Wikidata query interface, we are now ready to learn how we can embed Wikidata-driven maps in other Wikimedia projects, such as Wikipedia and Commons (see the example on the right). In addition to SPARQL we will look at GeoJson, OpenStreetMap and the Kartographer extentsion.
    Module 3 : Finally, and if times allows, we will have a look at the steps for creating fully interactive Wikidata-driven maps that can be used off-Wiki, ie. in regular HTML pages. In addtition to the above tools & techniques, we will use some basic Python, Jupyter Notebooks (PAWS), Jupyter-Leaflet and Jupyter-widgets.

Intended audiences

While this session is tech-focused and will discuss basic Wikidata techniques and programming tools, it is meant to be approachable by beginning Wikidatians and programmers. The workshop leader, by no means an advanced Python programmer nor Wikidatian himself, will be showing and sharing examples and code snippets that can be easily adapted by users with basic SPARQL and Python skills, to make them work for their own datasets.

As the workshop is comprised of three 30 minute modules, participants can decide to skip the modules that they find too advanced (or basic) for their individual knowledge levels.
Required preparations

In order to maximize the effective workshop time, participants are requested to do some preparations before coming to the workshop:

    Identify a geo-referenced set of coherent items in Wikidata to work with. Aim for 100-500 items or so.
    Create an account on Wikidata/ Wikimedia, if not yet done so.
    Set up a working PAWS notebook (Help 1, Help 2, Help 3) – only needed if the participant intends to follow Module 3

Relationship to the theme

This session will address the conference theme — Wikimedia, Free Knowledge and the Sustainable Development Goals — in the following manner:
Data visualisation is a key skill to learn (SGD 4) for people in today’s data-driven and visual societies. It helps to translate abstract, dry data - typically only understood by experts - into visual endproducts that can be understood by bigger audiences, thus helping to democratize knowledge and reduce inequalities (SDG 10).
Session outcomes

At the end of the session, attendees will:

    Understand the steps to make basic flat and layered maps in Wikidata, based on geo-referenced items and SPARQL queries (Level 1, basic)
    Understand the steps to embed these maps in Wikipedia, Wikimedia Commons and other Wikimedia sites (Level 2, intermediate)
    Understand the steps to create Wikidata-based maps than can be used in other (non-Wiki) websites (Level 3, advanced)
    Will have access to map making resources, SPARQL examples and Python code snippets they can build upon for their own projects after Wikimania.

Session leader(s)

    Olaf Janssen

Usernames

    OlafJanssen

Affiliation/country

    National library of The Netherlands & Wikimedia Netherlands

E-mail contact

    olaf.janssen@kb.nl

Session type

. The format of this submission is a:

    Computer-based training
    Workshop to identify and try to solve problem

Length of session

30/60/90 minutes, duration dependent on

    how much time the Space leaders are willing to provide
    how advanced & interactive participants will want to make the maps (see Levels 1,2 and 3 above, based on 30 minutes per level)

Please note that I proposed the same workshop in the GLAM Space on Friday and Saturday.
Supporting work

    Map materials for public libraries in The Netherlands - (work in progress)
    PAWS notebook for making off-wiki maps of public libraries in The Netherlands (work in progress)
    The map-related materials of User:Sic19, see map examples under Sparql-queries and GeoShapes

Requirements

The session will work best with these conditions:

    Room with projector for workshop leader. Wifi, seats, tables and wall outlets for participants bringing their laptops.
    Audience: 10-25 people, with basic knowledge about Wikidata, Sparql and Python (Jupyter Notebooks). Knowledge about GeoJson and OpenStreetMap will come in handy.
    Recording: Yes, recording allowed, happy to share knowledge

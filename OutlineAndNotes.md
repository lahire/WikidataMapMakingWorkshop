# Workshop outline and notes
*Last update: 10th August 2019*

## Module 1:  Basic flat & layered maps 

Prerequisites for this Module

* [Wikimedia account](https://www.wikidata.org/w/index.php?title=Special:CreateAccount)
* Working knowledge of [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page)
* Basic understanding of [SPARQL](https://en.wikipedia.org/wiki/SPARQL) and the [Wikidata Query Service](https://www.mediawiki.org/wiki/Wikidata_Query_Service/User_Manual) (WQS)
* A Wikidata set of items with geo coordinates [P625](https://www.wikidata.org/wiki/Property:P625)

If you do not have, or cannot create such a Wikidata set, you can use one of these: 
1) [Public libraries in The Netherlands](https://w.wiki/6dx) (incomplete set, per 10-8-2019)
2) [National heritage sites of the Netherlands](https://w.wiki/6dy) (limited to 1000 items)
3) [Big cities](https://w.wiki/6e3) in the world
4) [Volcanos](https://w.wiki/6e9)
5) [Airports around the equator](https://w.wiki/6eB) ( between -10 and +10 degrees latitude)
6) .... pick your own

Many examples in this workshop are based on the first dataset [Public libraries in The Netherlands](https://w.wiki/6dx)

### Module 1.1 Basic flat map
* [Public libraries in The Netherlands](https://w.wiki/6dx)
* [Default map view](https://w.wiki/6eq)
* Relation between query and popup
* [Hiding fields from popup](https://w.wiki/6mU)

### Module 1.2 Clustered flat map
* [Clustered flat map](https://w.wiki/6ew)

### Module 1.3 Basic layered map 
* [Dutch public libraries layered by province](https://w.wiki/6gJ) - Non-custom layer names = labels from Wikidata items 

### Module 1.4 Layered map, custom layer names 
* Libraries layered by postal code zone: https://bit.ly/3368DPk (do not click, copy-paste URL to browser)

### Module 1.5 Other cool layered maps 
* [Big cities, by population](https://w.wiki/3fx)
* [Disasters, by type](https://w.wiki/6gY)
* [Medieval churches, by century of construction](https://w.wiki/6ga)
* [Dutch municipalities, by number of public libraries](https://w.wiki/6gb)


## Module 2:  Embedded maps in Wikimedia projects

Prerequisites for this Module (in addtition to those in Module 1)
* User page on Wikipedia, Wikimedia Commons or Wikidata ([example](https://www.wikidata.org/wiki/User:OlafJanssen))... With [Sandbox](https://www.wikidata.org/wiki/User:OlafJanssen/Sandbox)

Nice to have some knowledge about 
* [OpenStreetMap](https://www.openstreetmap.org) (OSM)
* [GeoJSON](https://en.wikipedia.org/wiki/GeoJSON)

For embedding maps we'll be using the Mediawiki [Kartographer extension](https://www.mediawiki.org/wiki/Help:Extension:Kartographer)

All embedding examples below are available on https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019

### Basic map
* [Basic embedded map of The Netherlands](https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/0), without data. [View source](https://nl.wikipedia.org/w/index.php?title=Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019&action=edit&section=2)

### Module 2.1 Single location, hard-coded 
* [One public library in Amsterdam, geo coordinates hard-coded](https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/1). <sub>([View source](https://nl.wikipedia.org/w/index.php?title=Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019&action=edit&section=3))</sub> 
* Styling of markers https://github.com/mapbox/simplestyle-spec/tree/master/1.1.0#3-client-behavior and https://www.mediawiki.org/wiki/Help:Extension:Kartographer

### Module 2.2 Three locations, hard-coded 
* [Library, museum and archive in Amsterdam, geo coordinates hard-coded](https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/2). <sub>([View source](https://nl.wikipedia.org/w/index.php?title=Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019&action=edit&section=4))</sub> 

### Module 2.3 Outline (GeoShape) via Wikidata & OpenStreetMap 
* [Outline (geoshape) of Amsterdam public library (main site), using Wikidata and Open Street Map](https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/3). <sub>([View source](https://nl.wikipedia.org/w/index.php?title=Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019&action=edit&section=5))</sub>  
* [Wikidata item of Amsterdam Public Library, OBA Oosterdok (Centrale)](https://www.wikidata.org/wiki/Q50413436)
* [OBA Oosterdok on OSM](https://www.openstreetmap.org/way/240467636#map=19/52.37605/4.90853). Notice the Wikidata=Q50413436 in the tags on the left hand side.

### Module 2.4 Many locations, GeoJSON .map file 
* [Map of Dutch public libraries](https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/4). [View source](https://nl.wikipedia.org/w/index.php?title=Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019&action=edit&section=6)
* [.map file on Wikimedia Commons](https://commons.wikimedia.org/wiki/Data:DutchPublicLibraries.map). <sub>([View source](https://commons.wikimedia.org/w/index.php?title=Data:DutchPublicLibraries.map&action=edit))</sub>
* [Help: Map Data](https://www.mediawiki.org/wiki/Help:Map_Data)
* http://geojson.io
* SPARQL query to make .tsv file as input for Geojson.io: https://bit.ly/2YG48aY  (copy-paste URL to browser, do not click)

### Module 2.5 Combining data types 
* https://www.mediawiki.org/wiki/Help:Extension:Kartographer#Combining_multiple_data_types
* [Combining GeoShape (with geomask) and .map](https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/5). <sub>([View source](https://nl.wikipedia.org/w/index.php?title=Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019&action=edit&section=7))</sub>
* [Map of public libraries in the Dutch province of North-Holland](https://commons.wikimedia.org/wiki/Data:DutchPublicLibrariesNorthHolland.map)

### Module 2.6 GeoShapes using SPARQL and OSM
* https://www.mediawiki.org/wiki/Help:Extension:Kartographer#GeoShapes_via_Wikidata_Query
* [Maps with geoshapes based on SPARQL queries in Wikidata](https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/6). <sub>([View source](https://nl.wikipedia.org/w/index.php?title=Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019&action=edit&section=8))</sub>
* [GeoShape of Libya (Q1016)](https://www.openstreetmap.org/relation/192758#map=5/22.086/20.039) on OSM
* [SPARQL query to generate geoshapes of African countries](https://bit.ly/2YBxV4t)
* Variables must have names ?id ?title ?description ?fill ?stroke
* In the SPARQL query only use single quotes, otherwise you’ll get a JSON parse error

### Module 2.7 Other cool embedded maps
* [Railway lines around Klang Valley, Malaysia](https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/7).  <sub>([View source](https://nl.wikipedia.org/w/index.php?title=Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019&action=edit&section=9))</sub>
* [Governors of US states with their party affiliation](https://www.mediawiki.org/wiki/Help:Extension:Kartographer#/map/4) and  https://www.mediawiki.org/wiki/Help:Extension:Kartographer#GeoShapes_via_Wikidata_Query
* [Examples by Simon Cobb](https://www.wikidata.org/wiki/User:Sic19#GeoShapes)


## Module 3 : Off-wiki layered Wikidata-driven maps

Prerequisites (in addtition to those in Modules 1 and 2)
* Mediawiki account - https://www.mediawiki.org
Nice to have basic working knowledge about 
* Python
* PAWS / Jupyter Notebooks https://www.mediawiki.org/wiki/PAWS + https://realpython.com/jupyter-notebook-introduction/
Annd nice to have heard about 
* Jupyter-Leaflet https://github.com/jupyter-widgets/ipyleaflet + https://ipyleaflet.readthedocs.io/en/latest/
* Jupyter-widgets https://github.com/jupyter-widgets/ipywidgets + https://ipywidgets.readthedocs.io/en/latest/

### Module 3.1  Introduction to PAWS // Getting PAWS up and running
* PAWS homepage https://www.mediawiki.org/wiki/PAWS
* Starting your PAWS server https://paws.wmflabs.org/paws/hub + https://paws.wmflabs.org/paws/hub/user/USERNAME
* Running PAWS server https://paws.wmflabs.org/paws/user/USERNAME/tree
* PAWS terminal(s) https://paws.wmflabs.org/paws/user/USERNAME/terminals/1 (/2, /3, /4 etc for additional terminals)
* Stopping PAWS server https://paws.wmflabs.org/paws/hub/home
* PAWS public folder (even when server is offline) https://paws-public.wmflabs.org/paws-public/User:USERNAME

### Module 3.2  Installing example notebook
* Go to PAWS public folder of User:OlafJanssen https://paws-public.wmflabs.org/paws-public/User:OlafJanssen
* Save raw json file MapMakingWorkshop_Wikimania2019.ipynb to your PC https://paws-public.wmflabs.org/paws-public/User:OlafJanssen/MapMakingWorkshop_Wikimania2019.ipynb?format=raw
* Upload this json file to your own PAWS server
* Example notebook to play around with on your own server https://paws.wmflabs.org/paws/user/USERNAME/notebooks/MapMakingWorkshop_Wikimania2019.ipynb

### Module 3.3  Adapt example notebook, create your own interactive layered map
* Full instructions are given in the notebook. The notebook should be self-explanatory, so adapt, play, understand, get frustrated, learn.... Make your own interactive, layered map

### Module 3.4  Save your map for offline use
* Export the map to stand-alone off-Wiki HTML file  https://ipywidgets.readthedocs.io/en/latest/embedding.html#python-interface
* The addition of 'state=dependency_state([m])' keeps the html file growing too large
* Python code: embed_minimal_html('NetherlandsPublicLibrariesHeatmap.html', views=[m], state=dependency_state([m]), title='Heat map of Dutch public libraries, Wikimania map making workshop, 18th August 2019')


## END OF WORKSHOP


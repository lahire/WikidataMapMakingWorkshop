# Workshop outline and notes

Workshop description : https://wikimania.wikimedia.org/wiki/2019:Libraries/Map_making_workshop_%E2%80%93_from_Wikidata_to_interactive_off-wiki_maps_in_three_steps
Archived URL: https://web.archive.org/web/20190808101032/https://wikimania.wikimedia.org/wiki/2019:Libraries/Map_making_workshop_%E2%80%93_from_Wikidata_to_interactive_off-wiki_maps_in_three_steps

Full slides of workshop
* TO ADD on [Wikimedia Commons]()
* TO ADD on [Slideshare]()

==========================================================================

## Module 1:  Basic flat & layered maps 

Prerequisites (check with participants): 

* Wikimedia account
* Working knowledge of Wikidata
* Understanding of SPARQL
* A Wikidata set of items with geo coordinates (P625)….  https://www.wikidata.org/wiki/Property:P625
* … Or you can create one now

5-10 minutes : participants create SPARQL query to get set of items with geo coordinates --> provide assistance

If you do not have, or cannot create a Wikidata set of items with geo coordinates (P625), you can use one of these: 
1) Public libraries in The Netherlands : https://w.wiki/6dx
2) National heritage sites of the Netherlands: https://w.wiki/6dy
3) Big cities: https://w.wiki/6e3
4) Volcanos: https://w.wiki/6e9
5) Airports around the equator: https://w.wiki/6eB
6) .... pick your own

For the rest of the workshop I'll work with the first dataset (Public libraries in The Netherlands)

----- Module 1.1 Basic flat map -----
* Public libraries in The Netherlands https://w.wiki/6dx
* Default map view https://w.wiki/6eq
* Relation between query and popup
* Hiding fields from popup https://w.wiki/6mU

----- Module 1.2 Clustered flat map -----
* Clustered flat map https://w.wiki/6ew

----- Module 1.3 Basic layered map -----
* Libraries layered by province - Non-custom layer names = labels from WD-items https://w.wiki/6gJ

----- Module 1.4 Layered map, custom layer names -----
* Libraries layered by postal code zone <nowiki>https://bit.ly/3368DPk</nowiki> (copy-paste to browser, do not click)

----- Module 1.5 Other cool layered maps -----
* Big cities, by population https://w.wiki/3fx
* Disasters, by type https://w.wiki/6gY
* Medieval churches, by century of construction https://w.wiki/6ga
* Dutch municipalities, by number of public libraries https://w.wiki/6gb


## Module 2:  Embedded maps in Wikimedia projects

Prerequisites (in addtition to those in Module 1)
* User page on Wikipedia, Commons or Wikidata ...With Sandbox
Nice to have: some knowledge about 
* OpenStreetMap (OSM) https://www.openstreetmap.org
* GeoJSON https://en.wikipedia.org/wiki/GeoJSON

We'll be using the Kartographer extension : https://www.mediawiki.org/wiki/Help:Extension:Kartographer

The examples below are available on https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019

* Basic embedded map of The Netherlands https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/0

----- Module 2.1 Single location, hard-coded -----
* One public library in Amsterdam, geo coordinates hard-coded https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/1
* Styling of markers https://github.com/mapbox/simplestyle-spec/tree/master/1.1.0#3-client-behavior and https://www.mediawiki.org/wiki/Help:Extension:Kartographer

----- Module 2.2 Three locations, hard-coded -----
* Library, museum and archive in Amsterdam, geo coordinates hard-coded https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/2

----- Module 2.3 Outline (GeoShape) via Wikidata & OpenStreetMap -----
* Outline (geoshape) of Amsterdam public library (main site), using Wikidata and Open Street Map https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/3
* Amsterdam Public Library, OBA Oosterdok (Centrale) https://www.wikidata.org/wiki/Q50413436
* OBA Oosterdok on OSM https://www.openstreetmap.org/way/240467636#map=19/52.37605/4.90853

----- Module 2.4 Many locations, GeoJSON .map file -----
* Map of Dutch public libraries https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/4
* .map file on Wikimedia Commons https://commons.wikimedia.org/wiki/Data:DutchPublicLibraries.map
* Help: Map Data https://www.mediawiki.org/wiki/Help:Map_Data
* Geojson.io
* SPARQL query to make .tsv file as input for Geojson.io <nowiki>https://bit.ly/2YG48aY</nowiki>  (copy-paste to browser, do not click)

----- Module 2.5 Combining data types -----
* https://www.mediawiki.org/wiki/Help:Extension:Kartographer#Combining_multiple_data_types
* Combining geoshape (with geomask) and .map https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/5
* Map of public libraries in North-Holland https://commons.wikimedia.org/wiki/Data:DutchPublicLibrariesNorthHolland.map

----- Module 2.6 GeoShapes using SPARQL and OSM ------
* https://www.mediawiki.org/wiki/Help:Extension:Kartographer#GeoShapes_via_Wikidata_Query
* Maps with geoshapes based on SPARQL queries in Wikidata https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/6
* GeoShape of Libya (Q1016) https://www.openstreetmap.org/relation/192758#map=5/22.086/20.039
* SPARQL-query to generate geoshapes of African countries <nowiki>https://bit.ly/2YBxV4t</nowiki> 
* Variables must have names ?id ?title ?description ?fill ?stroke
* In the SPARQL query only use single quotes, otherwise you’ll get a JSON parse error

----- Module 2.7 Other cool embedded maps -----
* Railway lines around Klang Valley, Malaysia https://nl.wikipedia.org/wiki/Gebruiker:OlafJanssen/KladblokMapMakingWorkshopWM2019#/map/7
* Governors of US states with their party affiliation https://www.mediawiki.org/wiki/Help:Extension:Kartographer#/map/4 and  https://www.mediawiki.org/wiki/Help:Extension:Kartographer#GeoShapes_via_Wikidata_Query
* Examples by Simon Cobb https://www.wikidata.org/wiki/User:Sic19#GeoShapes


## Module 3 : Off-wiki layered Wikidata-driven maps

Prerequisites (in addtition to those in Modules 1 and 2)
* Mediawiki account - https://www.mediawiki.org
Nice to have basic working knowledge about 
* Python
* PAWS / Jupyter Notebooks https://www.mediawiki.org/wiki/PAWS + https://realpython.com/jupyter-notebook-introduction/
Annd nice to have heard about 
* Jupyter-Leaflet https://github.com/jupyter-widgets/ipyleaflet + https://ipyleaflet.readthedocs.io/en/latest/
* Jupyter-widgets https://github.com/jupyter-widgets/ipywidgets + https://ipywidgets.readthedocs.io/en/latest/

----- Module 3.1  Introduction to PAWS // Getting PAWS up and running-----
* PAWS homepage https://www.mediawiki.org/wiki/PAWS
* Starting your PAWS server https://paws.wmflabs.org/paws/hub + https://paws.wmflabs.org/paws/hub/user/USERNAME
* Running PAWS server https://paws.wmflabs.org/paws/user/USERNAME/tree
* PAWS terminal(s) https://paws.wmflabs.org/paws/user/USERNAME/terminals/1 (/2, /3, /4 etc for additional terminals)
* Stopping PAWS server https://paws.wmflabs.org/paws/hub/home
* PAWS public folder (even when server is offline) https://paws-public.wmflabs.org/paws-public/User:USERNAME

----- Module 3.2  Installing example notebook -----
* Go to PAWS public folder of User:OlafJanssen https://paws-public.wmflabs.org/paws-public/User:OlafJanssen
* Save raw json file MapMakingWorkshop_Wikimania2019.ipynb to your PC https://paws-public.wmflabs.org/paws-public/User:OlafJanssen/MapMakingWorkshop_Wikimania2019.ipynb?format=raw
* Upload this json file to your own PAWS server
* Example notebook to play around with on your own server https://paws.wmflabs.org/paws/user/USERNAME/notebooks/MapMakingWorkshop_Wikimania2019.ipynb

----- Module 3.3  Adapt example notebook, create your own interactive layered map  -----
* Full instructions are given in the notebook. The notebook should be self-explanatory, so adapt, play, understand, get frustrated, learn.... Make your own interactive, layered map

----- Module 3.4  Save your map for offline use -----
* Export the map to stand-alone off-Wiki HTML file  https://ipywidgets.readthedocs.io/en/latest/embedding.html#python-interface
* The addition of 'state=dependency_state([m])' keeps the html file growing too large
* Python code: embed_minimal_html('NetherlandsPublicLibrariesHeatmap.html', views=[m], state=dependency_state([m]), title='Heat map of Dutch public libraries, Wikimania map making workshop, 18th August 2019')


==== END OF WORKSHOP ====


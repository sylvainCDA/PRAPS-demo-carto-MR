# carto-iram
prochaines étapes :
- cluster en bleu
- geotiff en local?
- afficher des tuiles vectorielles et les styliser!
- outil de recherche marqueur
- geocodage

Server http :
(installer python)
cd C:\Users\scedat\Desktop\PRAPS_hydrogéol\_GIS_DATA\_Outils-carto-demo-MR\Leaflet_v2
python -m http.server
(ou python -m http.server 7800) pour utiliser le port 7800 au lieu du 8000

-------------------
qgis : editer les geométries et les exporter en geojson
hébergement des geojson sur github (ou sur postgis : génération de geojson à la volée? ou cron)
librairie d'affichage : maplibre
editeur de style en ligne : maputnik
basemaps tuiles vectorielles
editer les menus et la légendes et les popups

framework geojango? (postgis, requetes spatiales ect. ou geoext)


outil hydrogeol :
-fonds de carte : osm ou topo? flux tms
- zonages geojson : hébergé sur github (ou codé en javascript pour l'exemple)
- PoI : hébergé sur github (ou codé en javascript pour l'exemple) ou POSTGIS
- librairie maplibre ou leaflet
- affichage popup html : à construire avec les attributs du geojson
- requêtes spatiales : uniquement avec POSTGIS
- 


processus : 
-------------
zonage et poi sur google earth / qgis
retravail sur qgis : + données attributaires
export geojson
encodage json ou hebergement github ou dossier local
librairie mapbox-gl-leaflet pour utiliser leaflet et tous ses plugins + maplibre pour les tuiles vectorielles


sources de données carto :
fao: https://data.apps.fao.org/aquamaps/



pistes leaflet:
--------------
clustering leaflet : 
	https://www.datavis.fr/maps/leaflet-cluster
	https://github.com/Leaflet/Leaflet.markercluster#using-the-plugin
	https://leaflet.github.io/Leaflet.markercluster/example/marker-clustering-realworld.388.html
Geojson to Javascript : https://www.convertsimple.com/convert-json-to-javascript/
legende leaflet : 
	https://github.com/ptma/Leaflet.Legend
	https://codepen.io/haakseth/pen/KQbjdO
	https://gis.stackexchange.com/questions/133630/adding-leaflet-legend
masques leaflet : 
	https://github.com/ptma/Leaflet.Mask
	https://frogcat.github.io/leaflet-tilelayer-mask/
	http://jsfiddle.net/FranceImage/1yaqtx9u/
swipemap leaflet :
https://github.com/phloose/leaflet-compare --> https://phloose.github.io/leaflet-compare/
geotiff : 
https://github.com/stuartmatthews/leaflet-geotiff
AFFICHER DES FONDS DE PLAN HORS LIGNE : https://stackoverflow.com/questions/43743097/showing-an-offline-osm-map-file-suggestion-an-mb-tiles-file-with-js-library
Openmaptiles and leaflet : https://openmaptiles.org/docs/website/leaflet/


autres pistes :
---------------------
wms to tiles : https://github.com/lmikolajczak/wms-tiles-downloader
vector tiles : https://github.com/klokantech/vector-tiles-sample
télécharger des mbtiles : https://data.maptiler.com/downloads/africa/
charger geojson : https://stackoverflow.com/questions/66355293/leaflet-how-to-fetch-geojson-from-url-and-pass-it-to-l-geojson
charger des geojson, shapefiles à la volée : 
https://github.com/calvinmetcalf/leaflet.shapefile --> http://leaflet.calvinmetcalf.com


PLUGIN leaflet installés : 
clustering : https://github.com/Leaflet/Leaflet.markercluster
fullscreen : https://github.com/brunob/leaflet.fullscreen

PLUGIN leaflet à installer : 
geotiff : https://github.com/stuartmatthews/leaflet-geotiff
recherche dans les marqueurs leaflet : https://github.com/stefanocudini/leaflet-search  --> https://opengeo.tech/maps/leaflet-search/

pistes maplibre:
--------------
basemap maplibre : 
	https://github.com/ka7eh/maplibre-gl-basemaps
	https://gitlab.huma-num.fr/bmericskay/maplibre/-/blob/master/Basemapsmenu.html
swipemap maplibre :
	https://gitlab.huma-num.fr/bmericskay/maplibre/-/blob/master/Swipemap.html
legende maplibre : 
	https://gitlab.huma-num.fr/bmericskay/maplibre/-/blob/master/MaplibreFinal.html



------------
mémo :
* EPSG 4326 : WGS84 (elipsoide), lat/lon
* ESPG 3857 : WGS84/Web mercator, projection x y

MVT ou PBF??

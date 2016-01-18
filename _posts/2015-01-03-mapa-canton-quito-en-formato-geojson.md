---
layout:     post
title:      Mapa del cantón Quito en formato GeoJSON
date:       2015-01-03 21:30:00
summary:    This is an empty post to illustrate the pagination component with Pixyll.
categories: maps projects español
---

Comparto a continuación dos mapas de Quito en formato GeoJSON:

### Parroquias

Este archivo incluye los límites de las parroquias con información de la superficie, número de habitantes y la densidad de la población.

<script src="https://embed.github.com/view/geojson/flandrade/quito-crime-map/master/data/parroquias_quito.geojson"></script>

[DESCARGAR](https://raw.githubusercontent.com/flandrade/quito-crime-map/master/data/parroquias_quito.geojson)


### Administraciones zonales

Este archivo incluye los límites de las administraciones zonales con información del número de habitantes y densidad poblacional.

<script src="https://embed.github.com/view/geojson/flandrade/quito-crime-map/master/data/zonales_quito.geojson"></script>

[DESCARGAR](https://raw.githubusercontent.com/flandrade/quito-crime-map/master/data/zonales_quito.geojson)


El proceso de recopilación de información, sin embargo, estuvo lleno de contratiempos. Si bien el Municipio del Distrito de Quito ha compartido algunos datos, todavía queda un largo camino por recorrer. No basta con agregar información, sino que además es necesario verificar su formato de publicación.


## Desventajas de la información oficial disponible

El Municipio del Distrito de Quito publicó un portal de [Datos Abiertos](http://datosabiertos.quito.gob.ec/) en 2014. Esta página ofrece información relacionada a temas como educación, transporte, seguridad, demografía y territorio. Aquí se puede encontrar, por ejemplo, el promedio de personas que se [trasladan para trabajar](http://datos.quito.gob.ec/datastreams/141/promedio-de-personas-que-se-transladan-para-trabajar/) o el número de [robos a domicilios](http://datos.quito.gob.ec/datastreams/670/numero-de-denuncias-por-robos-a-domicilios-2015/) en 2015.

Esta iniciativa se integra a una política de trasparencia que ya ha sido implementada por diversos gobiernos de la región, entre ellos Colombia y México, pero es la primera en Ecuador. Pese a esto, se echa en falta el cuidado en el formato de publicación: es evidente que importaron los datos desde una hoja de cálculo. Por otro lado, no hay información geográfica detallada de la ciudad. Bastaría, de hecho, con un mapa sencillo, pero revisé todo el catálogo y no encontré ningún mapa que pueda ser utilizado directamente para una aplicación web.

De hecho, no encontré en ningún otro sitio un mapa de Quito en formato GeoJSON.

## Recopilación de información

El único mapa disponible en [Datos Abiertos](http://datosabiertos.quito.gob.ec/) de las administraciones zonales es un proyecto [ArcGIS](http://datosabiertos.quito.gob.ec/index.php/descargas). Fue necesario, por tanto, convertir estos archivos a GeoJSON a través de [shp2geojson.js](https://github.com/gipong/shp2geojson.js). Sin embargo, después de esta conversión, la ubicación de la ciudad no correspondía en el mapa de OpenStreetMap. Esto se solucionó actualizando las capas en [ArcGIS](https://www.arcgis.com/home/) en línea.

El mapa de las parroquias lo construí utilizando la información de [OpenStreetMap](http://wiki.openstreetmap.org/wiki/WikiProject_Ecuador). Los límites fueron creados a partir de las relaciones OSM (OpenStreetMap). Los polígonos (GeoJSON) fueron creados con [esta herramienta](http://polygons.openstreetmap.fr/index.py).

Finalmente, los datos de población y superficie fueron recopilados de [Ecuador en cifras](http://www.ecuadorencifras.gob.ec/informacion-censal-cantonal/) y [Datos Abiertos](http://datosabiertos.quito.gob.ec/).

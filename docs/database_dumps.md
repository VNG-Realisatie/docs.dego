---
layout: api-page-with-side-nav
title: Data Energie Gebouwde Omgeving (DEGO)
---

## Onze bronnen

Onze viewers gebruiken de onderstaande database bestanden.
Deze zijn grotendeels van andere publieke bronnen gedownload, en zelf verwerkt en opgemaakt. Voor de publieke bronnen, zie [Over onze data](/docs/metadata)

Dit zijn dus onze eigen verwerkte eindresultaten van wat er in de verschillende viewers te zien is.
De meest actuele data per gemeente kan via [csv](../csv) gedownload worden.


### Heel Nederland in 1 keer als data dump:

Voorbeeld met postgres inladen data van geopackage

Voer uit in de postgres database,  als de `postgis` extensie nog niet actief is.

    create extension postgis;

Daarna kun je de geopackage inladen.

    $ogr2ogr -f PostgreSQL 'PG:host=127.0.0.1 user=cdf dbname=cdf password=insecure'
     pand_energie_gegevens_nl.gpkg -lco OVERWRITE=YES



Download geopackage NL: [pand_energie_gegevens_nl.gpkg](https://files.commondatafactory.nl/dbdump/pand_energie_gegevens_nl.gpkg)

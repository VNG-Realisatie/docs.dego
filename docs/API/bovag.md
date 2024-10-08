---
layout: dego-page-with-side-nav
title: BOVAG API
---
Alle energie BOVAG geregistreerde bedrijven zijn op te vragen via de volgende API :


    https://ds.bovag.commondatafactory.nl/list/

De bedrijven zijn gekoppeld aan een bestaand BAG adres. Omdat de BOVAG niet een geldig BAG adres afdwingt hoeft dit dus niet overeen te komen. De `matchscore` geeft een indicatie in hoeverre het BOVAG adress overeenkomt met het dichtsbijzijnde BAG adres. 


### Beschrijving attributen

| attribuut            | beschrijving                                                                            | BRON        | Voorbeeld                                      |
| -------------------- | --------------------------------------------------------------------------------------- | ----------- | ---------------------------------------------- |
| id                   | volg ID                                                                                 |             | "1"                                            |
| vid                  | pand aanduiding ID                                                                      | BAG         | "0620100000001280"                             |
| sid                  | staanplaats aanduiding ID                                                               | BAG         | ""                                             |
| lid                  | ligplaats aanduiding ID                                                                 | BAG         | ""                                             |
| numid                | nummeraanduiding ID                                                                     | BAG         | "0620200000027486"                             |
| postcode             |                                                                                         | BAG         | "3769BV"                                       |
| huisnummer           |                                                                                         | BAG         | "5"                                            |
| huisletter           |                                                                                         | BAG         | ""                                             |
| huisnummertoevoeging |                                                                                         | BAG         | ""                                             |
| straat               |                                                                                         | RDW         | "SPORTLAAN"                                    |
| plaats               |                                                                                         | BAG         | "VIANEN"                                       |
| oppervlakte          | in m2                                                                                   | BAG         | "1381"                                         |
| geometry             | WKT xy coördinaten in WGS84                                                             | BAG         | "POINT (5.097708544646988 51.982227915259465)" |
| match_score          | match score waarop het BAG adres en BOVAG adres overeenkomen. Waarde 0 = correcte match | gegenereerd | "0"                                            |
| bag_toevoeging       |                                                                                         | BOVAG       | "25"                                           |
| lidid                |                                                                                         | BOVAG       | "2974700"                                      |
| bovag_toevoeging     |                                                                                         | BOVAG       | "25 "                                          |
| telephone            |                                                                                         | BOVAG       |                                                |
| emailaddress         |                                                                                         | BOVAG       |                                                |
| url                  |                                                                                         | BOVAG       |                                                |
| name                 |                                                                                         | BOVAG       |                                                |
| bovag_plaats         |                                                                                         | BOVAG       | "Soesterberg"                                  |
| bovag_postcode       |                                                                                         | BOVAG       | "3769 BV"                                      |
| bovag_adres          |                                                                                         | BOVAG       | "Postweg 25 "                                  |

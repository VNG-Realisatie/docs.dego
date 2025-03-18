---
title: "RDW API"
layout: api-page-with-side-nav
---



https://ds.rdw.commondatafactory.nl/list/


| attribuut            | beschrijving                                                                          | BRON        | Voorbeeld                                      |
| -------------------- | ------------------------------------------------------------------------------------- | ----------- | ---------------------------------------------- |
| id                   | volg ID                                                                               |             | "1"                                            |
| vid                  | pand aanduiding ID                                                                    | BAG         | "0620100000001280"                             |
| sid                  | staanplaats aanduiding ID                                                             | BAG         | ""                                             |
| lid                  | ligplaats aanduiding ID                                                               | BAG         | ""                                             |
| numid                | nummeraanduiding ID                                                                   | BAG         | "0620200000027486"                             |
| postcode             |                                                                                       | BAG         | "4131NN"                                       |
| huisnummer           |                                                                                       | BAG         | "5"                                            |
| huisletter           |                                                                                       | BAG         | ""                                             |
| huisnummertoevoeging |                                                                                       | BAG         | ""                                             |
| rdw_toevoeging       | RDW adres toevoeging                                                                  | RDW         | "5 "                                           |
| volgnummer           |                                                                                       | RDW         | "8286202"                                      |
| gevelnaam            |                                                                                       | RDW         | "Fabecars"                                     |
| naam_bedrijf         |                                                                                       | RDW         | "Fabecars B.V."                                |
| straat               |                                                                                       | RDW         | "SPORTLAAN"                                    |
| plaats               |                                                                                       | BAG         | "VIANEN"                                       |
| oppervlakte          | in m2                                                                                 | BAG         | "1381"                                         |
| geometry             | WKT xy coordinaten in WGS84                                                           | BAG         | "POINT (5.097708544646988 51.982227915259465)" |
| match_score          | match score waarop het BAG adres en RDW adres overeenkomen. Waarde 0 = correcte match | gegenereerd | "0"                                            |

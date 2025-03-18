---
title: API energie data
layout: api-page-with-side-nav
---
Alle energie data is per verblijfsobject op te vragen via de volgende API :

    https://ds.vboenergie.commondatafactory.nl/list/?match-gemeentecode=GM1680

(GM1680 = Aa en Hunze)

Webinterface:

    https://ds.vboenergie.commondatafactory.nl/

### Postman Collectie

[download postman collection](https://files.commondatafactory.nl/dbdump/CDF.postman_collection.json)

Deze API wordt gebruik in onze applicaties voor het optellen van de verblijfsobjecten, de aggregatie grafieken en de download functionaliteit.
Direct de API bevragen kan natuurlijk ook.

## Documentatie over filters en mogelijkheden kijk in de `help`:

    https://ds.vboenergie.commondatafactory.nl/help/

## API call Voorbeelden

Alle gegevens over een pand

    https://ds.vboenergie.commondatafactory.nl/list/?match-pid=1659100000000712

Zelfde als CSV

    https://ds.vboenergie.commondatafactory.nl/list/?match-pid=1659100000000712&format=csv

Alle addressen in buurt BU05184003 met energie klasse G als csv

    https://ds.vboenergie.commondatafactory.nl/list/?format=csv&match-buurtcode=BU05184003&match-energieklasse=G

Voorbeeld met python code en pandas.

    import pandas as pd
    data = pd.read_json('https://ds.vboenergie.commondatafactory.nl/list/?match-gemeentecode=GM0626')

De BRON is de open **kleinverbruik**
data, de verzameling open energie data
gepubliceerd door alle Nederlandse netbeheerders op postcode 6 niveau.

Mocht je nog vragen hebben. Email naar Verbeteren Informatie Positie - VIP @ vng .nl.

# Beschrijving attributen

| attribuut                      | beschrijving                                                                                                 | BRON           |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------ | -------------- |
| **numid**                      | Nummer aanduiding ID                                                                                         | BAG            |
| **pid**                        | Pand aanduiding ID                                                                                           | BAG            |
| **vid**                        | Verblijfsobject aanduiding ID                                                                                | BAG            |
| **lid**                        | Ligplaats aanduiding ID                                                                                      | BAG            |
| **sid**                        | Standplaats aanduiding ID                                                                                    | BAG            |
| **postcode**                   |                                                                                                              | BAG            |
| **straat**                     |                                                                                                              | BAG            |
| **huisnummer**                 |                                                                                                              | BAG            |
| **huisletter**                 |                                                                                                              | BAG            |
| **huisnummertoevoeging**       |                                                                                                              | BAG            |
| **oppervlakte**                |                                                                                                              | BAG            |
| **woningequivalent**           | Aantal Woning equivalenten per pand. 130 m² utiliteit staat gelijk aan 1 woningequivalent (weq). Een woning is ook gelijk aan 1 woningequivalent. | Berekening CDF |
| **gebruiksdoelen**             |                                                                                                              | BAG            |
| **pand_bouwjaar**              |                                                                                                              | BAG            |
| **gemiddelde_woz_waarde_woning**| Gemiddelde WOZ waarde in postcode gebied.  2022                                                             | CBS            |
| **gemiddelde_gemeente_woz**     | Gemiddelde WOZ waarde in gemeente van pand.  2022                                                           | CBS            |
| **pc6_eigendomssituatie_perc_koop**| Percentage koop woningen in postcode gebied                                                              | CBS            |
| **pc6_eigendomssituatie_perc_huur**| Percentage huur woningen in postcode gebied                                                              | CBS            |
| **pc6_eigendomssituatie_aantal_woningen_corporaties**| Percentage woningen in bezig van corporaties                                           | CBS            |
| **energieklasse**              | Energie label klasses A++++ tot G                                                                            | RVO            |
| **woning_type**                | Woning type uit energie labels                                                                               | RVO            |
| **pand_gebruiksoppervlakte**   |                                                                                                              | RVO            |
| **sbicode**                    | Afgeleid uit Energie label klasse                                                                            | RVO            |
| **gas_ean_count**              | Aantal gas aansluitingen per adres volgens EAN code boek                                                      | EAN Code boek  |
| **group_id_2022**              | Postcode 6 group ID over het jaar 2022.                                                                      | CDF            |
| **pc6_gasm3_2022**              | gemiddeld gas verbruik m3 in postcode 6 gebied over het jaar 2022                                            | kleinverbruik  |
| **pc6_kwh_2022**                | Gemiddeld elektra verbruik kwh in postcode 6 gebied                                                          | kleinverbruik  |
| **kwh_leveringsrichting_2022** | Met zonnepanelen is je leveringsrichting niet 100 van het net maar lager.                                    | kleinverbruik  |
| **pc6_grondbeslag_m2**          | Totaal oppervlakete op de grond van panden in postcode6 gebied van energie aggregatie.                       | BAG            |
| **pc6_gas_aansluitingen_2022**  | Aantal gas aansluitingen in het postcode 6 gebied volgens netbeheerder.                                      | kleinverbruik  |
| **point**                      | X Y coördinaten in WGS84                                                                                     | BAG            |
| **buurtcode**                  | buurt code volgens CBS                                                                                       | CBS            |
| **buurtnaam**                  | buurt naam volgens CBS                                                                                       | CBS            |
| **wijkcode**                   | wijk code volgens CBS                                                                                        | CBS            |
| **wijknaam**                   | wijk code volgens CBS                                                                                        | CBS            |
| **gemeentecode**               | gemeente code volgens CBS                                                                                    | CBS            |
| **gemeentenaam**               | gemeente code volgens CBS                                                                                    | CBS            |
| **provincienaam**              | province code volgens CBS                                                                                    | CBS            |
| **provinciecode**              | provincie code volgens CBS                                                                                   | CBS            |

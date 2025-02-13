---
layout: page-with-side-nav
title: Data Energie Gebouwde Omgeving (DEGO)
---

# Data bron omschrijving

De gebruikte data komt uit verscheidene bronnen en wij combineren het tot een mooi samenhangend geheel
waarmee u kunt werken. Bij alle bronnen staat een waarschuwing / disclaimer over het bestaan
van fouten:

### Disclaimer Bij Gebruik van deze internetsite

De databestanden die via deze internetsite aangeboden worden zijn bedoeld voor gebruik in
open data toepassingen en bevatten geen enkele interpretatie. De informatie kan niet worden
gebruikt in plaats van advies. Beslissingen op basis van deze informatie zijn voor uw eigen rekening en risico.
De open data op de commondatafactory.nl zijn met grote zorg samengesteld.
Desondanks kan geen enkele garantie gegeven worden met betrekking tot de volledigheid, juistheid of
actualiteit van de open data.


De gebruikte bronnen:

- [BAG-register van het Kadaster](https://data.nlextract.nl/bag/postgis/bag-laatst.backup),
- [3D BAG-data van TU Delft](http://3dbag.bk.tudelft.nl/downloads),
- [CBS Kerncijfers Wijken en Buurten](https://www.cbs.nl/nl-nl/reeksen/kerncijfers-wijken-en-buurten-2004-2020), maar wij gebruiken de Python API van het CBS hiervoor,
- [RVO energielabels](https://www.rvo.nl/onderwerpen/duurzaam-ondernemen/gebouwen/hulpmiddelen-tools-en-inspiratie-gebouwen/ep-online)
- kleinverbruiksdata van websites van de Nederlandse netbeheerders:
  - [Enexis](https://www.enexis.nl/over-ons/wat-bieden-we/andere-diensten/open-data)
  - [Liander](https://www.liander.nl/partners/datadiensten/open-data/data)
  - [Stedin](https://www.stedin.net/zakelijk/open-data/verbruiksgegevens)
  - [Rendo](https://www.rendonetwerken.nl/algemeen/opendata/disclaimer/beschikbare-data/)
  - [Enduris](https://www.rendonetwerken.nl/algemeen/opendata/disclaimer/beschikbare-data/)
  - [Coteq](https://coteqnetbeheer.nl/Over-Coteq/Open-data)
  - [Westland](https://www.westlandinfra.nl/over-westland-infra/open-data)

## Gecombineerde data.

De BAG en kleinverbruik gegevens zijn gecombineerd om voor een of meer postcode 6 gebieden een indicatie
van het verbruik per m2 en m3 volume gebouw. Het is een indicatie zoals een energie label over een
aantal panden samen. In de BAG, de kleinverbruik gegevens en pandhoogte zitten en kunnen fouten zitten
die elkaar versterken. De gegevens geven een goed beeld maar kunnen wel degelijk afwijken van de realiteit.

## Interpretatie valkuilen.

Gebouw combinaties die bij elkaar genomen zijn in een postcode 6 gebied zouden totaal niet handig zijn voor gelijk
tijdige aanpak of interpretatie van gegevens. Ze kunnen geografisch ver van elkaar liggen of van totaal andere tijden
en insolatie graden zijn. De viewers proberen inzicht te geven welke gegevens en gebouwen met elkaar gecombineerd zijn.

Het kan voorkomen dat in een postcode 6 gebied maar weinig gas aansluitingen zitten. Een nagenoeg all-electric wijk
kan door een paar niet zuinige gas aansluitingen toch heel hoog op de kaart komen voor het gasverbruik. Kijk dus
ook naar de aanwezige aansluitingen.

## Opmerkingen

Oude postcode 6 gebieden zijn vaak erg versnipperd en klein terwijl in nieuwbouw wijken postcode gebieden
doorgaans erg groot zijn. We hopen in de toekomst dat er een andere indeling wordt gebruik dan postcode 6
en zijn daarover in gesprek.

## Kwaliteit van de data
Ter verduidelijking hebben we per attribuut beschreven waar het vandaan wordt gehaald.
Daarnaast hebben we per attribuut vermeld hoeveel data er gemist wordt, indien er data gemist wordt.


Hieronder staan een aantal attributen waarop u moet letten qua datakwaliteit:

Dataset 	| Kolomnaam 	| Opmerking
---	| ---	| --:
BAG 	|   roof\_flat 	|   In ontwikkeling, precisie = 80%
Energy 	|   roof\_flat 	|  In ontwikkeling, precisie = 80%
Energy 	|   elabel\_definitief 	|  62% van de gebouwen heeft geen definitief energielabel gemeten
Energy 	|   elabel\_voorlopig 	|  11% van de gebouwen heeft geen voorlopig energielabel
Energy 	|   gasm3\_per\_m3 	|  24,23% data mist
CBS 	|   koopwoningen\_percentage 	|  21.41% data mist
CBS 	|   woningcorporatie\_woningen\_percentage 	|  21.41% data mist
CBS 	|   bouwjaar\_percentage\_voor2000 	|   21.27% data mist
CBS 	|   bedrijven\_per\_buurt 	|   29.93% data mist
CBS 	|   personenautos\_per\_huishouden 	|   20.81% data mist
CBS 	|   gasverbruik\_per\_huis\_gemiddeld 	|   19.10% data mist
CBS 	|   elektriciteitsverbruik\_per\_huis\_gemiddeld 	|   **100.00% data mist**
CBS 	|   adressen\_per\_km2 	|   37.99% data mist
CBS 	|   lagerinkomen\_percentage\_huishouden 	|   37.99% data mist
CBS 	|   hogerinkomen\_percentage\_huishouden 	|   86.35% data mist
CBS 	|   inkomen\_gemiddeld\_per\_inwoner 	|   **86.72% data mist**
CBS 	|   gasverbruik\_relatief\_aan\_inkomen 	|   **86.37% data mist**
CBS 	|   elekverbruik\_relatief\_aan\_inkomen 	|   20.86% data mist
CBS 	|   arbeidsongeschiktheid\_percentage 	|   **100.00% data mist**

---
title: WFS CBS data
layout: api-page-with-side-nav
---

Omdat een WFS zo handig is, en GIS-programma's al veel worden gebruikt in
gemeentes, willen wij u onze data ook aanbieden in dit formaat. Hierdoor kunt u
bijvoorbeeld data die alleen in uw gemeente beschikbaar is eenvoudig toevoegen,
en filteren op eigenschappen van buurten.

## WebFeature Services (WFS)

WebFeature Services, afgekort WFS, zijn niet meer weg te denken uit als geo data voorzienning.
Met WFS onsloten datasets kunnen op vele manieren worden opgevraagd en gebruikt
te visualiseren en te verwerken.

Een WFS bevat altijd een geografische component, en is daarom ideaal
voor projecten zoals de transitievisie warmte. Voorbeelden van programma's om
een WFS mee te openen zijn ArcGis en QGIS.


##  CBS data WFS

[maps.commondatafactory.nl/maps/cbs/](https://maps.commondatafactory.nl/maps/cbs?service=WFS&request=Getcapabilities)

#### Hoe gebruikt u onze WFS?
De link die u hierboven ziet, kopieert en plakt u naar uw favoriete
GIS-programma op de plek waar u een WFS kunt inladen. Als de WFS is geladen,
kunt u de dataset kiezen die u wilt zien op de kaart.
Daarna kunt u uw gewenste styling eraan geven om de belangrijke informatie te laten opvallen.

Als dit problemen oplevert, kunt u ook kiezen voor het
[kant-en-klaar qgis project](/docs/gis)
dat is gemaakt voor QGIS. Dit hoeft u
alleen te openen met een GIS-programma en dan staat alles klaar om te
gebruiken.

Bij vragen kom op de slack #datafactory https://samenorganiseren.slack.com



## Beschrijving attributen - CBS WFS 

De data is beschikbaar op buurt , wijk en gemeente niveau. 

| attribuut                              | beschrijving | BRON |
| -------------------------------------- | ------------ | ---- |
| buurtnaam                              |              | CBS  |
| buurtcode                              |              | CBS  |
| wijknaam                               |              | CBS  |
| wijkcode                               |              | CBS  |
| gemeentenaam                           |              | CBS  |
| gemeentecode                           |              | CBS  |
| omgevingsadressendichtheid             |              | CBS  |
| stedelijkheid_adressen_per_km2         |              | CBS  |
| bevolkingsdichtheid_inwoners_per_km2   |              | CBS  |
| aantal_huishoudens                     |              | CBS  |
| aantal_inwoners                        |              | CBS  |
| gemiddelde_huishoudsgrootte            |              | CBS  |
| percentage_personen_0_tot_15_jaar      |              | CBS  |
| percentage_personen_15_tot_25_jaar     |              | CBS  |
| percentage_personen_25_tot_45_jaar     |              | CBS  |
| percentage_personen_45_tot_65_jaar     |              | CBS  |
| percentage_personen_65_jaar_en_ouder   |              | CBS  |
| percentage_eenpersoonshuishoudens      |              | CBS  |
| percentage_huishoudens_zonder_kinderen |              | CBS  |
| percentage_huishoudens_met_kinderen    |              | CBS  |
| provincienaam                          |              | CBS  |
| provinciecode                          |              | CBS  |

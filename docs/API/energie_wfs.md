---
title: "WFS Energietransitie"
path: "/docs/energie/wfs"
---

Omdat een WFS zo handig is, en GIS-programma's al veel worden gebruikt in
gemeentes, willen wij u onze data ook aanbieden in dit formaat. Hierdoor kunt u
bijvoorbeeld data die alleen in uw gemeente beschikbaar is eenvoudig toevoegen,
en filteren op eigenschappen van buurten.
We hebben een WFS voor elk van de volgende categorieën:

## WebFeature Services (WFS)

WebFeature Services, afgekort WFS, zijn niet meer weg te denken uit als geo data voorzienning.
Met WFS onsloten datasets kunnen op vele manieren worden opgevraagd en gebruikt
te visualiseren en te verwerken.

Een WFS bevat altijd een geografische component, en is daarom ideaal
voor projecten zoals de transitievisie warmte. Voorbeelden van programma's om
een WFS mee te openen zijn ArcGis en QGIS.

## energie data per gebouw WFS

[maps.commondatafactory.nl/maps/energy](https://maps.commondatafactory.nl/maps/energy?service=WFS&request=Getcapabilities)


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



## Beschrijving attributen - Energie WFS 

Deze dataset is samengesteld uit open-data bronnen
van netbeheerders (2014 tot nu) , de Basis Administratie Gebouwen
en eancodeboek.nl. Ook bag3d (tu-delft) is gebruikt voor hoogte data.

Dit is een zogenaamde 'convenience' dataset samengesteld van beschikbare
open bronnen.

Een aantal attributen zijn zelf samengesteld [cdf].


### Basis 

| attribuut     | beschrijving                                        | BRON   |
| ------------- | --------------------------------------------------- | ------ |
| gid           |                                                     |        |
| identificatie |                                                     |        |
| gemeentecode  |                                                     | BAG    |
| tile_id       |                                                     | CDF    |
| bouwjaar      |                                                     | BAG    |
| m2            |                                                     |        |
| hoogte        | BAG 3D hoogte. 50 percentiel van laser punt meting. | BAG 3D |
|               |                                                     |        |


Enegie data wordt per postcode gebied gepubliceerd. Met
het `group_id` is te achterhalen welke panden bij elkaar
horen. Dit kan helaas per jaar verschillend.

| attribuut      | beschrijving | BRON |
| -------------- | ------------ | ---- |
| group_id_2014  |              | CDF  |
| group_id_2015  |              | CDF  |
| group_id_2016  |              | CDF  |
| group_id_2017  |              | CDF  |
| group_id_2018  |              | CDF  |
| group_id_2019  |              | CDF  |
| group_id_2020  |              | CDF  |
| pandcount_2014 |              | CDF  |
| pandcount_2015 |              | CDF  |
| pandcount_2016 |              | CDF  |
| pandcount_2017 |              | CDF  |
| pandcount_2018 |              | CDF  |
| pandcount_2019 |              | CDF  |
| pandcount_2020 |              | CDF  |

### Energie verbruik per jaar.

2020 is peildatum 01-01-2020 dus gaat over jaar 2019.
vanaf 2020 is teruglevering los van verbruik genomen
voor 2020 werd teruglevering van het gebruik afgetrokken.

Beschikbare elektra verbruiks gegevens per postcode 6

| attribuut                  | beschrijving                                               | BRON                        |
| -------------------------- | ---------------------------------------------------------- | --------------------------- |
| gasm3_2020                 |                                                            | kleinverbruik netbeheerders |
| gasm3_2019                 |                                                            | kleinverbruik netbeheerders |
| gasm3_2018                 |                                                            | kleinverbruik netbeheerders |
| gasm3_2017                 |                                                            | kleinverbruik netbeheerders |
| gasm3_2016                 |                                                            | kleinverbruik netbeheerders |
| gasm3_2015                 |                                                            | kleinverbruik netbeheerders |
| gasm3_2014                 |                                                            | kleinverbruik netbeheerders |
| kwh_2014                   |                                                            | kleinverbruik netbeheerders |
| kwh_2015                   |                                                            | kleinverbruik netbeheerders |
| kwh_2016                   |                                                            | kleinverbruik netbeheerders |
| kwh_2017                   |                                                            | kleinverbruik netbeheerders |
| kwh_2018                   |                                                            | kleinverbruik netbeheerders |
| kwh_2019                   |                                                            | kleinverbruik netbeheerders |
| kwh_2020                   |                                                            | kleinverbruik netbeheerders |
| gas_aansluitingen_2014     | Aantal gas aansluitingen in postcode 6 gebied              | kleinverbruik netbeheerders |
| gas_aansluitingen_2015     | Aantal gas aansluitingen in postcode 6 gebied              | kleinverbruik netbeheerders |
| gas_aansluitingen_2016     | Aantal gas aansluitingen in postcode 6 gebied              | kleinverbruik netbeheerders |
| gas_aansluitingen_2017     | Aantal gas aansluitingen in postcode 6 gebied              | kleinverbruik netbeheerders |
| gas_aansluitingen_2018     | Aantal gas aansluitingen in postcode 6 gebied              | kleinverbruik netbeheerders |
| gas_aansluitingen_2019     | Aantal gas aansluitingen in postcode 6 gebied              | kleinverbruik netbeheerders |
| gas_aansluitingen_2020     | Aantal gas aansluitingen in postcode 6 gebied              | kleinverbruik netbeheerders |
| gas_pct_2014               | Percentage panden in postcode 6 gebied met gas aansluiting | kleinverbruik netbeheerders |
| gas_pct_2015               | Percentage panden in postcode 6 gebied met gas aansluiting | kleinverbruik netbeheerders |
| gas_pct_2016               | Percentage panden in postcode 6 gebied met gas aansluiting | kleinverbruik netbeheerders |
| gas_pct_2017               | Percentage panden in postcode 6 gebied met gas aansluiting | kleinverbruik netbeheerders |
| gas_pct_2018               | Percentage panden in postcode 6 gebied met gas aansluiting | kleinverbruik netbeheerders |
| gas_pct_2019               | Percentage panden in postcode 6 gebied met gas aansluiting | kleinverbruik netbeheerders |
| gas_pct_2020               | Percentage panden in postcode 6 gebied met gas aansluiting | kleinverbruik netbeheerders |
| kwh_aansluitingen_2014     |                                                            | kleinverbruik netbeheerders |
| kwh_aansluitingen_2015     |                                                            | kleinverbruik netbeheerders |
| kwh_aansluitingen_2016     |                                                            | kleinverbruik netbeheerders |
| kwh_aansluitingen_2017     |                                                            | kleinverbruik netbeheerders |
| kwh_aansluitingen_2018     |                                                            | kleinverbruik netbeheerders |
| kwh_aansluitingen_2019     |                                                            | kleinverbruik netbeheerders |
| kwh_aansluitingen_2020     |                                                            | kleinverbruik netbeheerders |
| kwh_leveringsrichting_2014 |                                                            | kleinverbruik netbeheerders |
| kwh_leveringsrichting_2015 |                                                            | kleinverbruik netbeheerders |
| kwh_leveringsrichting_2016 |                                                            | kleinverbruik netbeheerders |
| kwh_leveringsrichting_2017 |                                                            | kleinverbruik netbeheerders |
| kwh_leveringsrichting_2018 |                                                            | kleinverbruik netbeheerders |
| kwh_leveringsrichting_2019 |                                                            | kleinverbruik netbeheerders |
| kwh_leveringsrichting_2020 |                                                            | kleinverbruik netbeheerders |

Teruglevering indicatie. Een waarde lager dan 100 betekent dat
er energie terug wordt geleverd aan het net en geeft
aan dat er waarschijnlijk zonnepanelen aanwezig zijn.


| attribuut                  | beschrijving | BRON |
| -------------------------- | ------------ | ---- |
| kwh_leveringsrichting_2020 |              |      |
| kwh_leveringsrichting_2019 |              |      |
| kwh_leveringsrichting_2018 |              |      |
| kwh_leveringsrichting_2017 |              |      |
| kwh_leveringsrichting_2016 |              |      |
| kwh_leveringsrichting_2015 |              |      |
| kwh_leveringsrichting_2014 |              |      |

ean_code_count | | EAN Code boek | 


Energie label voorlopig / Definitief. Bron RVO.

- `elabel_voorlopig`
- `elabel_definitief`


Poging om een trend uit te rekenen van de beschikbare  data. Wordt niet getoont in de viewer. 

- `kwh_trend`,
- `gasm3_trend`
- `gasm3_std`
- `gas_pct_trend`,
- `gas_pct_std`,
- `kwh_leveringsrichting_trend`
- `kwh_leveringsrichting_std`

## Energie afgeleide indicatoren

Onderstaande indicatoren zijn berekend maar erg fout
gevoelig door fouten in meetwaarden en onduidelijkheid
welke panden in een postcode gebied zitten. Schuurtjes worden
niet meegenomen bijvoorbeeld maar dit zal niet altijd goed zijn.

De hoogte kan door bewolking tijdens satellietmeting in
grote gebieden niet goed doorkomen.

Indicatie van het totaal gas verbruik per m3 in pc6 gebied
= gemiddelde * aantal aansluitingen.

- `totaal_verbruik_m3`,

Een opsomming van het totaal volume aanwezig in panden
volgens panden * m2 * bag3d hoogte.

- `totaal_volume_m3`
- `totaal_oppervlak_m2`

Gasverbruik afgezet tegen het totaal aantal m2 pand beslag.
Dus niet de vloeren.

- `gasm3_per_m2`

Gasverbruik afgezet tegen het totaal aantal m3 in de betrokken
panden in een postcode 6 gebied.

- `gasm3_per_m3`

- `bouwjaar`


Aantal gas aansluitingen volgens het eancodeboek.nl in het pand.
Dit gaat fout in de aanwezigheid van toevoegingen want het
EAN codeboek volgt niet altijd de bag. Dit is verder wel de meest
precieze indicatie die we hebben voor de aanwezigheid van een
gasaansluiting.

- `ean_code_count`


## BAG 3D informatie 


| attribuut     | beschrijving | BRON   |
| ------------- | ------------ | ------ |
| nr_ground_pts |              | BAG 3D |
| nr_roof_pts   |              | BAG 3D |
| ground-0.00   |              | BAG 3D |
| ground-0.10   |              | BAG 3D |
| ground-0.20   |              | BAG 3D |
| ground-0.30   |              | BAG 3D |
| ground-0.40   |              | BAG 3D |
| ground-0.50   |              | BAG 3D |
| rmse-0.25     |              | BAG 3D |
| rmse-0.50     |              | BAG 3D |
| rmse-0.75     |              | BAG 3D |
| rmse-0.90     |              | BAG 3D |
| rmse-0.95     |              | BAG 3D |
| rmse-0.99     |              | BAG 3D |
| roof_flat     |              | BAG 3D |
| roof-0.25     |              | BAG 3D |
| roof-0.50     |              | BAG 3D |
| roof-0.75     |              | BAG 3D |
| roof-0.90     |              | BAG 3D |
| roof-0.95     |              | BAG 3D |
| roof-0.99     |              | BAG 3D |
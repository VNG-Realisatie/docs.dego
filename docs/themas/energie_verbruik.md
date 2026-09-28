---
title: "Energie verbruik"
layout: thema-page-with-side-nav
datum: 26-07-2026
---
## Energieverbruik

Inzicht in het gemiddelde gas- en elektriciteitsverbruik per huishouden, gasverbruik per m² en de teruglevering, kan gemeenten helpen om meer zicht te krijgen of een gebied veel, weinig of gemiddeld gasverbruik heeft . Dit kan iets zeggen over de energetische kwaliteit van gebouwen en mogelijk ook over het stookgedrag van inwoners.   

### Gasverbruik 2024
Het gasverbruik geeft aan hoeveel aardgas een object verbruikt, in m3 per jaar. Het verbruik wordt weergegeven per postcodegebied en alleen als een pand daadwerkelijk een gasaansluiting heeft. Met deze inzichten kun je – indien gewenst – bepalen wat de CO2- reductie is als het object overgaat naar een aardgasvrije warmtevoorziening.

Het gasverbruik per vierkante meter grondbeslag (oppervlak zonder verdiepingen) geeft een indicatie van de relatieve energiezuinigheid van panden. Een hoog gasverbruik kan immers veroorzaakt worden door een slechte isolatie, maar ook door de grootte van een pand of omdat er bedrijvigheid is die veel gas nodig heeft. Als het gasverbruik per m2 grondbeslag laag is, wordt er dus relatief efficiënt verwarmd. Het grondbeslag is berekend op basis van de polygonen uit de BAG. 

Het gasverbruik per kubieke meter object geeft een indicatie van de energiezuinigheid van een object. Een hoog gasverbruik kan immers veroorzaakt worden door slechte isolatie, maar ook doordat een object erg groot is. De hoogte van een pand komt uit de BAG3D van TU-delft met behulp van laser metingen. Helaas is niet van elk pand een hoogte beschikbaar. Samen met het feit dat kleinverbruik gegevens over meerdere panden gaat, zitten er grote gaten in de kaart. De kaart lijkt overeen te komen met de m2 laag maar in hoogbouw zijn toch aanzienlijke verschillen te zien.

Bij de berekening van het gemiddelde aardgasverbruik zijn woningen met een zeer laag of zelfs nulverbruik meegeteld indien er sprake is van stadsverwarming. Hierdoor valt in gebieden waar stadsverwarming aanwezig is het gemiddelde aardgasverbruik per woningen laag uit.


_Bron: Kleinverbruik bestanden van alle netbeheerders_<br/>
_Bron: BAG (voor de oppervlakte)_<br/>
_Bron: BAG3D TU Delft (voor hoogte pand)_<br/>
_Update: Jaarlijks_<br/>
_Niveau: per postcode 6 gebied_<br/>


### Elektriciteitsverbruik 2024
Het elektriciteitsverbruik geeft aan hoeveel elektriciteit een object verbruikt, in kWh per jaar. Het verbruik wordt weergegeven per postcodegebied. Met deze inzichten kun je bepalen welke gebieden er gemiddeld veel of weinig elektriciteit verbruiken.

Collectieve elektriciteitsleveringen aan bijvoorbeeld liftinstallaties of hal-/galerijverlichting zijn niet meegeteld bij de berekening

_Bron: Kleinverbruik bestanden van alle netbeheerders_<br/>
_Update: Jaarlijks_<br/>
_Niveau: per postcode 6 gebied_<br/>

#### Verwerking van kleinverbruikgegevens
De bestanden van de energieleveranciers hebben verschillende structuren en bevatten overlappende postcodegebieden. Daarom moet de data eerst worden opgeschoond en geharmoniseerd voordat deze kan worden gebruikt.
De belangrijkste bewerkingen zijn:
-	Postcodes: Als alleen postcode_van bekend is, wordt deze ook als postcode_tot gebruikt. Duitse postcodes bij Enexis en Liander worden verwijderd; bij een combinatie van Nederlandse en Duitse postcodes wordt alleen de Nederlandse postcode gebruikt. 
-	SJA: Decimale waarden worden afgerond naar beneden door alleen het gehele deel te behouden. 
-	Kleine gebieden: Werkgebieden met minder dan één aansluiting per postcode worden verwijderd als ze geen overlap hebben met een significant gebied. 
-	Overlappende gebieden: Bij overlap wordt een gebied met minder dan één aansluiting per postcode verwijderd. Bij gedeeltelijke overlap die niet betrouwbaar kan worden opgelost, wordt het minst significante gebied verwijderd. 
-	Moeder- en kindgebieden: Gebieden die volledig binnen een groter gebied vallen, worden samengevoegd. De gegevens worden daarbij gecombineerd tot één moedergebied, met een nieuw gewogen gemiddelde. Ook worden de unieke leveranciersnamen samengevoegd. 


Kortom: de data wordt eerst gestandaardiseerd, opgeschoond en ontdubbeld, waarna overlappende en geneste werkgebieden worden samengevoegd tot een zo betrouwbaar mogelijk eindresultaat.



### Gemiddeld verbruik per buurt, uitgesplitst naar huur en koop
Binnen een wijk kunnen er grote verschillen zitten tussen de energieverbruiken van huur en koopwoningen. Deze kaartlaag toont een uitsplitsing naar huur en koopwoningen van het energieverbruik op buurtniveau. Als er grote verschillen in energieverbruik zijn tussen huur en koop, kan dit invloed hebben op de wijkaanpak.

Bij uitgesplitst naar huur en koop wordt er onderscheid gemaakt tussen:

-	Gemiddeld gasverbruik huurwoning
-	Gemiddeld gasverbruik koopwoning
-	Gemiddeld elektriciteitsverbruik huurwoning
-	Gemiddeld elektriciteitsverbruik koopwoning
-	Gemiddeld elektriciteitsverbruik totaal

_Bron: CBS, kerncijfers wijken en buurten_<br/>
_Update: Jaarlijks_<br/>
_Niveau: per gemeente, wijk, buurt_<br/>



---
title: "API SBI codes"
layout: dego-page-with-side-nav
---

Alle Standaard Bedrijfs Indeling codes (SBIcodes) zijn op te vragen via de volgende API:

    https://ds.sbicodes.commondatafactory.nl/list/?format=csv

Webinterface:

    https://ds.sbicodes.commondatafactory.nl/

Vrijzoeken

    https://ds.sbicodes.commondatafactory.nl/v0/search?search=koolzaad

Bron: sbi.cbs.nl.

Deze API wordt gebruik in onze applicaties voor het zoeken en fileren
van sbicodes op categorien.

Documentatie over filters en mogelijkheden kijk in de `help`:

    https://ds.sbicodes.commondatafactory.nl/help/

Voorbeelden:

Alle gegevens over een pand

    https://ds.sbicodes.commondatafactory.nl/v0/list?match-code=01

Zelfde als CSV

    https://ds.sbicodes.commondatafactory.nl/v0/list?match-code=01&format=csv

Or met startswith

    https://ds.sbicodes.commondatafactory.nl/v0/list?startswith-code=01&format=csv


Voorbeeld met python code en pandas.

    import pandas as pd
    data = pd.read_json('https://ds.sbicodes.commondatafactory.nl/v0/list')

Mocht je nog vragen hebben. Email naar Verbeteren Informatie Positie - VIP @ vng .nl.

De sbicodes zijn ingedeel in 2 hierarchien.  1e is de hierarchie met codes die van
01 - 011 - 0113 - 01131 gaat als voorbeeld.

De andere hierarchie is gebaseerd op vraag antwoord systeem.
Bouw - Vraag 2 - Vraag 3. Niet alle codes hebben een plek in het vraag systeem.

Gebruikt door dego.vng.nl en dook.vng.nl.

# Beschrijving attributen

| attribuut                      | beschrijving                                                                                                 | BRON           |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------ | -------------- |
| **code**                       | SBI Code.                                                                                                    | sbi.cbs.nl     |
| **omschrijving**               | Omschijving SBI Code.
| **l1**                         | Hooffcategorie, A, B C...
| **l1d**                        | Omschijving
| **l2**                         | Niveau 2 in hierarchie
| **l2d**                        | Omschijving
| **l3**                         | Niveau 3 in hierarchie
| **l3d**                        | Omschrijving
| **l4**                         | Niveau 4 in hierarchie
| **l4d**                        | Omschijving
| **l5**                         | Niveau 5 in hierarchie
| **l5d**                        | Omschrijving
| **q1**                         | Vraag 1 van sbi.cbs.nl
| **q2**                         | Vraag 2 in sbi.cbs.nl
| **q3**                         | Vraag 3 in sbi.cbs.nl
| **description**                | Vraag 3 in sbi.cbs.nl




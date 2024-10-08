---
title: "KVK download beschrijving "
layout: dego-page-with-side-nav
---


| attribuut            | beschrijving | BRON | 
| -------------------- | ------------ | ---- | 
| numid                |              | BAG  |
| straat               |              | BAG  |
| huisnummer           |              | BAG  |
| huisletter           |              | BAG  |
| huisnummertoevoeging |              | BAG  |
| postcode             |              | BAG  |
| gemeentenaam         |              | BAG  |
| gebruiksdoelen       |              | BAG  |
| oppervlakte          |              | BAG  |
| pand_bouwjaar        |              | BAG  |


| attribuut                             | beschrijving | BRON | 
| ------------------------------------- | ------------ | ---- | 
| KVK_Handelsnaam                       |              | KVK     |
| KVK_Nummer                            |              | KVK     |
| KVK_Bedrijfsactiviteit                |              | KVK     |
| KVK_SBI_code                          |              | KVK     |
| KVK_SBI_code_hoofdactiviteit          |              | KVK     |
| KVK_SBI_omschrijving_hoofdact         |              | KVK     |
| KVK_SBI_code_nevenactiviteit1         |              | KVK     |
| KVK_SBI_omschrijving_nevenactiviteit1 |              | KVK     |
| KVK_SBI_code_nevenactiviteit2         |              | KVK     |
| KVK_SBI_omschrijving_nevenactiviteit2 |              | KVK     |
| KVK_Rechtsvorm                        |              | KVK     |
| KVK_Datum_inschrijving_onderneming    |              | KVK     |
| KVK_Datum_uitschrijving_onderneming   |              | KVK     |
| KVK_Vestigingsnummer                  |              | KVK     |
| KVK_Datum_inschrijving_vestiging      |              | KVK     |
| KVK_Datum_uitschrijving_vestiging     |              | KVK     |
| KVK_Indicatiehoofdvestiging           |              | KVK     |

### Bedrijventereinen specifiek 


| attribuut                             | beschrijving                         | BRON        | 
| ------------------------------------- | ------------------------------------ | ----------- | 
| Indicatie_bedrijf_aanwezig_op_adres   | Aantal bedrijven aanwezig op adres   | gegenereerd |
| Indicatie_stichting_aanwezig_op_adres | Aantal Stichtingen aanwezig op adres | gegenereerd |


### Autobranche specifiek 



| attribuut                    | beschrijving                                                                                             | BRON        | 
| ---------------------------- | -------------------------------------------------------------------------------------------------------- | ----------- | 
| indicatie_RDW_erkenning      | Aantal RDW erkenningen aanwezig op adres                                                                 | gegenereerd |
| indicatie_BOVAG_lidmaatschap | Aantal BOVAG erkenningen aanwezig op adres                                                               | gegenereerd |
| indicatie_KVK_autobranche    | Aantal KVK autobranche bedrijven aanwezig op adres                                                       | gegenereerd |
| rdw_volgnummer               | ID nummer van RDW dataset                                                                                | RDW         |
| rdw_naam_bedrijf             |                                                                                                          | RDW         |
| rdw_gevelnaam                |                                                                                                          | RDW         |
| rdw_erkenningen              | Array met voorkomende RDW erkenningen                                                                    | RDW         |
| rdw_matchscore               | Match score waarop RDW adres overeenkomt met BAG adres. Een score van 0 betekend perfecte overeenkomst   | RDW         |
| rdw_toevoeging               | RDW adres nummer toevoeging                                                                              | RDW         |
| bovag_naam                   |                                                                                                          | BOVAG       |
| bovag_adres                  | Adres zoals in BOVAG gegevens staat aangeduid                                                            | BOVAG       |
| bovag_matchscore             | Match score waarop BOVAG adres overeenkomt met BAG adres. Een score van 0 betekend perfecte overeenkomst | BOVAG       |

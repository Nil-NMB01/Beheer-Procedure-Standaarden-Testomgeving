# Beheerproces NLGOV standaarden onder MIDO Governance

Dit document geeft het beheerproces voor standaarden in hoofdlijnen weer voor goedkeuring van NLGOV Standaarden i.c.m. MIDO Governance.
De NLGOV Standaarden worden door Logius beheerd volgens [Beheermodellen](https://github.com/Logius-standaarden) gebaseerd op [BOMOS](https://www.logius.nl/domeinen/infrastructuur/bomos) 

In de onderstaande hoofdstukken wordt ingegaan op het RFC Proces voor het verwerken van wijzigingsvoorstellen, het Release planningsproces en het Release proces.


## RFC (Request for Change)  Proces 

Een binnen gekomen wijzigingsvoorstel wordt door Beheer beoordeeld en voorgelegd aan het Technisch Overleg (of direct aan een hoger MIDO gremium als het voorstel een tactisch / strategisch vraagstuk betreft).

In het Technisch Overleg wordt het wijzingsvoorstel besproken en beoordeeld (het voorstel kan indien nodig ook door het Technich Overleg worden voorgelegd aan de MIDO Programmeringstafel).
Als het voorstel wordt goedgekeurd wordt het voorstel door Beheer indien nodig verder uitgewerkt, vervolgens wordt het voorstel door Beheer ter Goedkeuring voorgelegd aan het Technisch Overleg.

> _NB De Stuurgroep Kennisplatform API's wordt geinformeeerd over ontwikkelingen mbt binnen het platform ontwikkelde standaarden, de besluitvorming vindt plaats in het MIDO_

Het onderstaande schema geeft het proces mbt beoordelen van wijzigingsvoorstellen in hoofdlijnen weer:

![Alt text](./media/mido_rfc_release_rfc.svg)

[Legenda](#bijlage-bpmn-legenda)



|Activiteit | Verantwoordelijk | Toelichting | RFC status (begin)| RFC status (eind)
|----|----|----|---|---|
|Intake RFC|Beheer|Beheer legt issue voor aan TO of hoger Gremium | - | ter Beoordeling|
|Beoordelen_RFC|TO / Progr. tafel / Progr. Raad|Het Gremium beoordeelt het issue en geeft aan of dit moet worden uitgewerkt|ter Beoordeling | in Bewerking |
|Uitwerken|Beheer| Uitwerking RFC  |in Bewerking | ter Goedkeuring|
|Beoordelen|TO | Het TO beoordeelt de uitwerking en geeft aan of de RFC moet worden doorgevoerd |ter Goedkeuring | Gereed |
|Doorvoeren RFC| Beheer|  Beheer voert de RFC door  |Gereed  | Klaar voor release|


## Release Planning Proces

In het Release Planning Proces worden de goedgekeurde Wijzigingsvoorstellen opgenomen in een bepaalde release van de standaard. Beheer doet hier een voorstel voor en het Releaseplan wordt afgestemd binnen het Technisch Overleg en de MIDO Programmeringstafel; Het Releaseplan geeft aan welke wijzigingen in de eerstvolgende release worden opgenomen en welke in een latere release van de de standaard. 

Het onderstaande schema geeft het Release Planning Proces in hoofdlijnen weer:

<img src="./media/mido_releaseplan.svg" width="70%" alt="Description of the release plan image">

[Legenda](#bijlage-bpmn-legenda)

|Activiteit | Verantwoordelijk | Toelichting | Releaseplan status (begin)|  Releaseplan status (eind)|
|----|----|----|---|---|
|Opstellen Releaseplan voorstel|Beheer | Goedgekeurde RFC's worden gebundeld in een voorstel voor een nieuwe release van de standaard| - |ter Beoordeling|
|Beoordelen Releaseplan voorstel|TO|Het TO beoordeelt het releaseplan |ter Beoordeling | TO:Goedgekeurd
|Beoordelen Releaseplan voorstel| Programmeringstafel| Programmeringstafel beoordeelt het releaseplan |TO:Goedgekeurd | PT:Goedgekeurd
|Publiceren Releaseplan | Beheer| releaseplan wordt gepubliceerd| PT:Goedgekeurd | Gepubliceerd|

> _NB Het Releaseplan wordt aan de Programmeringstafel ter beoordeling aangeboden wanneer het plan tactische/strategische vragen met zich mee brengt_

## Release Proces

In het Releaseproces wordt een volgende release van de standaard samengesteld door Beheer conform het Releaseplan.
De nieuwe versie wordt vervolgens publiek geconsulteerd, en de resultaten van de consultatie worden besproken in het Technisch Overleg en verwerkt. De definitieve release wordt vervolgens voor vaststelling geagendeerd bij de MIDO Programmeringstafel (bij een major/minor wijziging) en bij de Programmeringsraad (alleen bij major wijzigingen). 
Na Goedkeuring wordt de standaard door Beheer gepubliceerd.


![Alt text](./media/mido_rfc_release_kpapi.svg)


[Legenda](#bijlage-bpmn-legenda)

|Activiteit | Verantwoordelijk | Toelichting | Release status (begin) | Release status (eind)| Release status (document) |
|----|----|----|---| ---|---|
|Samenstellen_Release|Beheer | Conform de releaseplanning worden goedgekeurde RFC's gebundeld in een nieuwe release van de standaard | - |in Consultatie | __Document:__ Consultatie versie <BR> __Governance:__ _|
|Publieke_Consultatie|Beheer| De Release wordt publiek geconsulteerd en reacties worden verzameld en voorgelegd aan TO |in Consultatie | ter Goedkeuring| __Document:__ Consultatie versie <BR> __Governance:__ _|
|Beoordelen Consultatie|TO| Het TO beoordeelt de resultaten van de consultatie en geeft aan welke eventuele aanpassingen nodig zijn |ter Goedkeuring | TO:Release_ Goedgekeurd| __Document:__ Consultatie versie <BR> __Governance:__ TO:Release_Goedgekeurd
|Samenstellen Definitieve Release | Beheer | Samenstellen definitieve release | TO:Release_ Goedgekeurd | ter Vaststelling|__Document:__ Versie ter vaststelling <BR> __Governance:__ TO:Release_Goedgekeurd |
|Agenderen Release | Beheer   | Agenderen MIDO | ter Vaststelling | ter Vaststelling |__Document:__ Versie ter vaststelling  <BR> __Governance:__  TO:Release_Goedgekeurd <BR>| 
|Goedkeuren Release | MIDO Programmerings tafel  |Beoordelen release (major/minor) - minor versies worden door de programmeringstafel vastgesteld, major versies gaan bij een posititief advies van de tafel door naar de programmeringsraad voor vaststelling | (ter Vaststelling) TO:Release_ Goedgekeurd | PT:Release_ Goedgekeurd  | __Document:__ Versie ter vaststelling  <BR> __Governance:__  TO:Release_Goedgekeurd <BR> PT:Release_Goedgekeurd | 
|Goedkeuren Release | MIDO Programmerings raad |Beoordelen release (major) | (ter Vaststelling) PT:Release_ Goedgekeurd | PR:Release_ Goedgekeurd| __Document:__ Versie ter vaststelling  <BR> __Governance:__  TO:Release_Goedgekeurd <BR> PT:Release_ Goedgekeurd <BR> PR:Release_ Goedgekeurd |  |
|Publicatie | Beheer | Publiceren van de release en release notes | PT/PR:Release_ Goedgekeurd | Vastgesteld | __Document:__ Vastgesteld  <BR> __Governance:__  TO:Release_Goedgekeurd <BR>  PT:Release_Goedgekeurd <BR> PR:Release_Goedgekeurd | 

## SOTD voorbeeld:

Zie als voorbeeld van de State of this document de onderstaande tabel:

| Organization / Committee                                     | Version number                                               | Official status                                              | Date       |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ---------- |
| [Forum Standaardisatie](https://www.forumstandaardisatie.nl/open-standaarden/rest-api-design-rules) | [1.0]( https://gitdocumentatie.logius.nl/publicatie/api/adr/1.0) | reported                                                     | 15-10-2019 |
| [Forum Standaardisatie](https://www.forumstandaardisatie.nl/open-standaarden/rest-api-design-rules) | [1.0]( https://gitdocumentatie.logius.nl/publicatie/api/adr/1.0) | ['comply of explain' standard (mandatory open standard)](https://gitdocumentatie.logius.nl/publicatie/api/adr/) | 09-07-2020 |
| [Working group](https://github.com/Geonovum/KP-APIs/tree/03d7fd61b3f25eef5d3242c7beee688e0d2d9623/overleggen/Werkgroep%20API%20design%20rules/Verslagen/20230905) | [2.0.0-rc.1](https://gitdocumentatie.logius.nl/publicatie/api/adr/2.0.0-rc.1/) | working version / final draft by 'Working Group'             | 05-09-2023 |
| [KP API Steering committee](https://github.com/Geonovum/KP-APIs/tree/master/overleggen/Stuurgroep/Verslagen) | [2.0.0-rc.1](https://gitdocumentatie.logius.nl/publicatie/api/adr/2.0.0-rc.1/) | approved consultation version / adopted by 'KP API'          | 21-09-2024 |
| [MIDO programmeringstafel](https://pgdi.nl/groups/view/c9a77467-7118-42c4-ad27-d0da773bc7dc/programmeringstafels-en-financiele-commissie-pgdi/files/82ac7589-ce2a-4c39-aabd-99eb9a6cf43a) | [2.0.0-rc.2](https://gitdocumentatie.logius.nl/publicatie/api/adr/2.0.0-rc.2) | release candidate 2 / definitief concept                     | 14-02-2024 |
| [MIDO PGDI Committee](https://pgdi.nl/groups/view/fa975d80-05e2-4f9e-89d6-6a053295c97b/programmeringsraad-gdi/files) | [2.0.0-rc.2](https://gitdocumentatie.logius.nl/publicatie/api/adr/2.0.0-rc.2) | definitive version / approved by 'PGDI'                      | 07-03-2024 |
| [Forum Standaardisatie](https://www.forumstandaardisatie.nl/open-standaarden/rest-api-design-rules) | [2.0.0-rc.2](https://gitdocumentatie.logius.nl/publicatie/api/adr/2.0.0-rc.2) | reported                                                     | 25-01-2024 |
| [Forum Standaardisatie](https://www.forumstandaardisatie.nl/open-standaarden/rest-api-design-rules) | [2.0.0](https://gitdocumentatie.logius.nl/publicatie/api/adr/2.0.0) | intake pending                                               | 18-04-2024 |
| [Forum Standaardisatie](https://www.forumstandaardisatie.nl/open-standaarden/rest-api-design-rules) | [2.0.0](https://gitdocumentatie.logius.nl/publicatie/api/adr/2.0.0) | definitive version / approved by Forum Standaardisatie       | tbd        |



## Bijlage Begrippenlijst

### 1. Gremium
**Gremium**: Een formeel overlegorgaan of comité waarin beslissingen worden genomen of adviezen worden gegeven over specifieke onderwerpen, in deze context de besluitvorming en coordinatie rondom de infrastructuur en digitale ontwikkeling van de Digitale Overheid.

### 2. KPAPI (Kennisplatform API)
**KPAPI (Kennisplatform API)**: Het Kennisplatform API is een open platform, waar overheden, marktpartijen, gebruikers en aanbieders samen werken aan een Nederlandse API strategie en alles wat daarbij komt kijken. Hiernaast is er ook een stuurgroep van deze platform en die heeft een adviserende rol in geval van de normatieve standaarden die onder MIDO governance vallen. De stuurgroep wordt geinformeerd over ontwikkelingen en de besluitvorming vind vervolgens plaats in het MIDO.

### 3. Major change
**Major change**: Een major change is een grote wijziging en wordt bij de definitieve release voor vaststelling zowel geagendeerd bij de MIDO Programmeringstafel als bij de MIDO Programmeringsraad. Grote wijzigingen worden alleen geagendeerd bij de Programmeringsraad en kleine wijzigingen niet (minor changes).

### 4. MIDO (Meerjarenprogramma Infrastructuur Digitale Overheid)
**MIDO (Meerjarenprogramma Infrastructuur Digitale Overheid)**: Het MIDO is een samenwerkingsprogramma van overheden en publieke dienstverleners dat gericht is op de modernisering en gezamenlijke governance van de Generieke Digitale Infrastructuur (GDI), met als doel veilige, toegankelijke en betrouwbare digitale publieke dienstverlening te waarborgen.

### 5. MIDO Programmeringstafel
**MIDO Programmeringstafel**: Het programmeringstafel is een inhoudelijke voorbereiding, overleg en afstemming van plannen tussen betrokken partijen binnen het MIDO programma.

### 6. MIDO Programmeringsraad
**MIDO Programmeringsraad**: De programmeringsraad is een beslissend orgaan, waarin de strategische besluitvorming en goedkeuring van plannen en dergelijke dingen plaatsvinden binnen het MIDO programma.

### 7. Minor change
**Minor change**: Een minor change is een kleine wijziging en wordt bij de definitieve release voor vaststelling alleen geagendeerd bij het MIDO Programmeringstafel.

### 8. Release planningsproces
**Release planningsproces**: In het Release Planning Proces worden de goedgekeurde Wijzigingsvoorstellen opgenomen in een bepaalde release van de standaard.

### 9. Release proces
**Release proces**: In het Releaseproces wordt een volgende release van de standaard samengesteld door Beheer conform het Releaseplan.

### 10. RFC (Request for Change)
**RFC (Request for Change)**: Het RFC is een binnen gekomen wijzigingsvoorstel dat door Beheer wordt beoordeeld en voorgelegd aan het Technisch Overleg (of direct aan een hoger Stuurgroep/MIDO gremium als het voorstel een tactisch / strategisch vraagstuk betreft).

### 11. TO (Technisch Overleg)
**TO (Technisch Overleg)**: Het technisch overleg bespreekt actuele vraagstukken en ontwikkelingen rondom een bepaald standaard en beoordeelt wijzigingen aan de standaard. 

## Bijlage Statussen


### RFC Status

|Status  | Toelichting | 
|----|----|
| Afgewezen | Het voorstel is afgewezen en kan opnieuw in behandeling worden genomen na aanpassing. |
| Gereed | Het voorstel is aangenomen en kan worden doorgevoerd. |
| In bewerking | Het voorstel is in bewerking bij de beheerorganisatie.| 
| In onderzoek | Ter voorbereiding van uitwerking is onderzoek nodig. |
| Klaar voor release | Het voorstel is verwerkt en klaar voor de volgende release.|
| Ter goedkeuring | Het voorstel is uitgewerkt en wordt ter goedkeuring aangeboden.|
| Uitwerking door derden | Het voorstel wacht op uitwerking door een externe partij. |
> Zie ook [https://github.com/Logius-standaarden/Digikoppeling-Algemeen/labels](https://github.com/Logius-standaarden/Digikoppeling-Algemeen/labels)

### Release Status

|Status  | Toelichting | 
|----|----|
| in Consultatie | Release aangeboden voor consultatie |
| ter Goedkeuring | Release aangeboden voor Goedkeuring |
| TO:Release_ Goedgekeurd | Release goedgekeurd door TO |
| ter Vaststelling | Release aangeboden voor vaststelling |
| PT:Release_ Goedgekeurd | Release goedgekeurd door Programmeringstafel |
| PR:Release_ Goedgekeurd | Release goedgekeurd door Programmeringsraad |
| Vastgesteld | Release vastgesteld |


## Bijlage BPMN Legenda

![Legenda](./media/BPMN%20Symbolen%20afbeelding.PNG)



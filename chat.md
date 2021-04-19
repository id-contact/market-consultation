# ID Chat

Een typische ID Chat-plugin werkt als volgt. Een inwoner opent de webpagina van de gemeente en kiest het gewenste kanaal en de gewenste authenticatiemethode. In dit geval kiest de inwoner voor ‘veilig chatten’. De inwoner doorloopt het authenticatieproces en geeft toestemming om bepaalde attributen (persoonlijke gegevens) te delen met de gemeente. Hoe dit authenticatieproces precies verloopt, hangt af van de gekozen authenticatiemethode en is niet van belang voor de ID bellen-plugin. Deze persoonlijke gegevens worden kortstondig opgeslagen op de backend van ID Chat-plugin met als enige doel om ze aan de agent te tonen bij het aannemen van de sessie. Het platform herkent de chattende inwoner en routeert deze naar een beschikbare KCC Agent. Bij deze agent worden de gegevens van de inwoner getoond op het scherm. 

Kort samengevat is de functie van de gevraagde ID Chat-plugin:
- Het ontvangen en controleren van de attributen en kortstondig opslaan.
- Het verwijzen van de inwoner naar een omgeving waarbinnen met de KCC-agent gechat kan worden.
- De attributen tonen op het scherm van de KCC Agent.

Er is een Proof of Concept gerealiseerd, waarbij een ID Chat-plugin is gebouwd op basis van het opensource platform Matrix voor demonstratiedoeleinden. Deze plugin is als voorbeeld te gebruiken van een specifieke manier om een ID Chat-plugin op te zetten, maar per platform zal de architectuur wezenlijk kunnen verschillen. De beschrijving van deze plugin komt in een aantal weken beschikbaar op GitHub. Op de kortere termijn komt hier de beschrijving van een communicatie testplugin beschikbaar evenals de beschrijving van de ID Contact Core. 

## Introductievragen (te ontvangen voor 30 april, zie [Reageren op deze marktverkenning](./reactions.md))

1. Geef een korte beschrijving van je organisatie. Geef daarbij minimaal aan: *naam van de organisatie, vestigingsplaats, grootte van de organisatie, core business, aantal jaren actief in de markt.*
2. Geef een overzicht van de belangrijkste klanten waar jullie actief zijn. Geef daarbij minimaal aan: *een overzicht van alle gemeentelijke en andere (semi-)overheidsorganisaties*
3. Geef aan voor welk kanaal/welke kanalen jullie een plugin zouden willen/kunnen bouwen en voor welk product dit zou zijn.
4. Geef een beschrijving van jullie ontwikkelervaring en -capaciteit en slagkracht. Geef daarbij minimaal aan: *In hoeverre ontwikkelen jullie zelf of werken jullie samen met een partner of fabrikant? Geef voorbeelden van een ontwikkelde (API)koppeling of koppelingen.*

## Inhoudelijke vragen (te ontvangen voor 14 mei, zie [Reageren op deze marktverkenning](./reactions.md))
1. Graag lezen we jullie visie op ID Contact in het algemeen en ID Chat in het bijzonder.
2. We vragen je om ons inzicht te geven in de bouw van een ID Chat-plugin naar analogie van de plugin met Matrix zoals die hierboven is beschreven (als onderdeel van de PoC).
    - Lever een uitgewerkt technisch ontwerp voor een plugin. Wat zijn daarbij de randvoorwaarden? Denk daarbij aan de (infrastructurele) randvoorwaarden aan de gemeentekant. Maar ook aan de minimale uitgangspunten mbt jullie product, zoals aanwezige deelproducten/modules, softwarereleases etc. Hoe wordt ervoor gezorgd dat (bijzondere) persoonsgegevens zodanig worden verwerkt dat deze voldoen aan de eisen die eraan worden gesteld voor overheden?
    - Wat zijn de eenmalige kosten voor het daadwerkelijk bouwen van een plugin (waarbij de randvoorwaarden als een gegeven beschouwd mogen worden)?
    - Wat is een reële doorlooptijd voor het bouwen van een dergelijke plugin?
    - Geef een indicatie van jullie commerciële prijsvoering richting iedere organisatie die wil aansluiten obv jullie product.
3. De plugin zoals gebouwd in de PoC is het resultaat van een aantal ontwerpkeuzes. Wellicht biedt jullie platform mogelijkheden die een nieuw licht werpen op het ontwerp. Dan nodigen we jullie van harte uit om deze met ons te delen. We zitten nu in de fase dat er in de basis nog aanpassingen kunnen plaatsvinden. En deze alternatieven en verbetervoorstellen leveren ons ook inzichten op als het gaat om guidelines (UX, security etc) die we daarbij moeten opstellen/bewaken in fase II van het project.

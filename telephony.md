# ID Bellen

Een typische flow voor een ID Bellen- plugin verloopt als volgt: 

*Een inwoner opent de webpagina van de gemeente en kiest het gewenste kanaal en de gewenste authenticatiemethode. In dit geval kiest de inwoner voor ‘veilig bellen’. De inwoner doorloopt het authenticatieproces en geeft toestemming om bepaalde attributen (persoonlijke gegevens) te delen met de gemeente. Hoe dit authenticatieproces precies verloopt, hangt af van de gekozen authenticatiemethode en is niet van belang voor de ID bellen-plugin. De persoonlijke gegevens van de inwoner worden kortstondig opgeslagen op de backend van ID Contact met als enige doel om ze later aan een agent te tonen bij het aannemen van de sessie. Een dtmf generator in ID Contact zorgt voor een code en koppelt deze aan de op de backend opgeslagen attributen. Op de backend wordt deze dtmf code direct ingewisseld voor een session secret. Deze secret is dermate sterk dat hij onmogelijk geraden kan worden door derden. De inwoner ziet het telefoonnummer dat hij moet bellen evenals de dtmf code*. Via het telefoonnummer komt de beller binnen op het platform van de integratiepartner. Het platform ontvangt de code verifieert deze door de ID bellen-plugin te raadplegen. Indien de code niet correct is, wordt de inwoner gevraagd deze opnieuw in te toetsen. Indien de code correct is, wordt de beller in de wachtrij geplaatst. Zodra een KCC agent beschikbaar is, wordt de inwoner naar deze agent gerouteerd, wordt het bijbehorende secret opgehaald en worden de gegevens van de inwoner getoond op het scherm van de agent.*

**Hierbij zijn er twee varianten te onderscheiden: 1. De inwoner ziet het telefoonnummer en de dtmf code op zijn computer en wordt door het platform van de integratiepartner gevraagd de code in te toetsen. 2. De inwoner laadt (bijv via een QR code zowel telefoonnummer) als (komma-gescheiden) dmtf code direct in de native dialer van zijn mobiele telefoon.*

Kort samengevat is de functie van de gevraagde ID Bellen-plugin:

- Het ontvangen en controleren van de dtmf code en daarop acteren
- Het ophalen van de session secret op de backend van ID Contact, gegeven deze dtmf code
- De attributen tonen op het scherm van de KCC Agent, gegeven de opgehaalde session secret

Voor de Proof of Concept is een open source ID Bellen-plugin gebouwd op basis van het platform Amazon Connect (voor bellen). De beschrijving en de broncode van deze plugin zijn beschikbaar op [GitHub](https://github.com/id-contact/comm-amazon-connect), evenals de beschrijvingen en broncode van een [communicatie-testplugin](https://github.com/id-contact/comm-test), een [authenticatie-testplugin](https://github.com/id-contact/auth-test) en een beschrijving met broncode van de [ID Contact Core](https://github.com/id-contact/core). Op de wat langere termijn komen hier ook de beschrijvingen van de communicatie-plugin op basis van Matrix (voor chat) en de authenticatie-plugin voor IRMA.

## Introductievragen (te ontvangen voor 30 april, zie [Reageren op deze marktverkenning](./reactions.md))

1. Geef een korte beschrijving van je organisatie. Geef daarbij minimaal aan: *naam van de organisatie, vestigingsplaats, grootte van de organisatie, core business, aantal jaren actief in de markt.*

2. Geef een overzicht van de belangrijkste klanten waar jullie actief zijn. Geef daarbij minimaal aan: *een overzicht van alle gemeentelijke en andere (semi-)overheidsorganisaties.*

3. Geef aan voor welk kanaal/welke kanalen jullie een plugin zouden willen/kunnen bouwen en voor welk product dit zou zijn.

4. Geef een beschrijving van jullie ontwikkelervaring en -capaciteit en slagkracht. Geef daarbij minimaal aan: *In hoeverre ontwikkelen jullie zelf of werken jullie samen met een partner of fabrikant? Geef voorbeelden van een ontwikkelde (API)koppeling of koppelingen.*

## Inhoudelijke vragen (te ontvangen voor 14 mei, zie [Reageren op deze marktverkenning](./reactions.md))

1. Graag lezen we jullie visie op ID Contact in het algemeen en ID Bellen in het bijzonder.

2. We vragen je om ons inzicht te geven in de bouw van een ID Bellen-plugin naar analogie van de plugin zoals die hierboven is beschreven (als onderdeel van de PoC).

    -  Lever een visie op de uitwerking van het technisch ontwerp voor een plugin in Powerpoint, Visio of Miro.. Wat zijn daarbij de randvoorwaarden? Denk daarbij aan de (infrastructurele) randvoorwaarden aan de gemeentekant. Maar ook aan de minimale uitgangspunten m.b.t. jullie product, zoals aanwezige deelproducten/modules, softwarereleases etc. Hoe wordt ervoor gezorgd dat (bijzondere) persoonsgegevens zodanig worden verwerkt dat deze voldoen aan de eisen die eraan worden gesteld voor overheden?
    -  Wat zijn de eenmalige kosten voor het daadwerkelijk bouwen van een plugin zoals beschreven in bovenstaand technisch ontwerp? (waarbij de randvoorwaarden als een gegeven beschouwd mogen worden)?
    -  Wat is een reële doorlooptijd voor het bouwen van een dergelijke plugin?
    -  Geef een indicatie van jullie commerciële prijsvoering richting iedere organisatie die wil aansluiten obv jullie product

3. De plugin zoals gebouwd in de PoC met Amazon Connect is het resultaat van een aantal weloverwogen ontwerpkeuzes waarbij met name informatieveiligheid voorop stond. Wellicht biedt jullie platform mogelijkheden die een nieuw licht werpen op het ontwerp. Dan nodigen we jullie van harte uit om deze met ons te delen. We zitten nu in de fase dat er in de basis nog aanpassingen kunnen plaatsvinden. En deze alternatieven en verbetervoorstellen leveren ons ook inzichten op als het gaat om guidelines (UI, security etc) die we daarbij moeten opstellen/bewaken in fase II van het project.
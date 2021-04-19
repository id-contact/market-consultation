# ID Video

Er is nog geen werkende communicatie ID Video-plugin ontwikkeld voor de Proof of Concept. De werking van ID Video die we voor ogen hebben bestaat uit twee mogelijke varianten:

Variant 1: *Een inwoner kiest op de webpagina van de gemeente voor een product en kiest op betreffende webpagina het gewenste kanaal. In dit geval kiest de inwoner voor ‘veilig videobellen’. De inwoner krijgt een scherm waarin hij een afspraak kan maken (keuze datum/tijdstip) voor een videogesprek. Hij ontvangt een bevestigingse-mail met een link. De afspraak wordt eveneens bij een medewerker van de gemeente aangekondigd/ingepland. Tijdens het videogesprek wordt gekeken of authenticatie noodzakelijk is (afhankelijk van inhoud gesprek). De inwoner ziet dan een pop-up verschijnen waarin de beschikbare authenticatiemethoden worden gepresenteerd. Na het kiezen van een authenticatiemethode, wordt de inwoner ge-redirect en geeft deze toestemming om bepaalde gegevens (attributen) te delen. Deze attributen worden kortstondig op de backend van ID Contact opgeslagen met als enige doel om ze aan de agent te tonen wanneer de inwoner terugkeert naar het videogesprek. Nadat de gebruiker authenticatie doorlopen heeft, wordt deze teruggestuurd naar het videogesprek en worden de attributen aan de gemeentemedewerker getoond.*

Variant 2: *Een inwoner belt naar de gemeente. Daar blijkt dat middels een videogesprek met een medewerker de vraag kan worden beantwoord/de gewenste transactie kan worden voltooid. De KCC-medewerker plant een ‘veilig videobellen’ sessie in. De rest van de flow is gelijk aan variant 1.*

Kort samengevat is de functie van de gevraagde ID Video-plugin:
- Het tonen van een afsprakenmodule (direct aan inwoner via website of aan KCC-medewerker).
- Het creëren van een link die toegang geeft tot de sessie
- Het gedurende de sessie openen van een pop-up met een redirect naar de gekozen authenticatiemethode.
- Het ontvangen en controleren van de attributen en kortstondig opslaan.
- Het tonen van de attributen op het scherm van de gemeentemedewerker.

## Introductievragen (te ontvangen voor 30 april, zie [Reageren op deze marktverkenning](./reactions.md)).

1. Geef een korte beschrijving van je organisatie. Geef daarbij minimaal aan: *naam van de organisatie, vestigingsplaats, grootte van de organisatie, core business, aantal jaren actief in de markt.*

2. Geef een overzicht van de belangrijkste klanten waar jullie actief zijn. Geef daarbij minimaal aan: *een overzicht van alle gemeentelijke en andere (semi-)overheidsorganisaties*

3. Geef aan voor welk kanaal/welke kanalen jullie een plugin zouden willen/kunnen bouwen en voor welk product dit zou zijn.

4. Geef een beschrijving van jullie ontwikkelervaring en -capaciteit en slagkracht. Geef daarbij minimaal aan: *In hoeverre ontwikkelen jullie zelf of werken jullie samen met een partner of fabrikant? Geef voorbeelden van een ontwikkelde (API)koppeling of koppelingen.*

## Inhoudelijke vragen (te ontvangen voor 14 mei, zie [Reageren op deze marktverkenning](./reactions.md))

1. Graag lezen we jullie visie op ID Contact in het algemeen en ID Video in het bijzonder

2. We vragen je om ons inzicht te geven in de bouw van een mogelijk ID Video-plugin 
    - Beschrijf de werking van een mogelijke communicatie plugin voor ID Video. Welke stappen doorlopen daarbij zowel de inwoner als de medewerker van de gemeente?
    - Lever een uitgewerkt technisch ontwerp voor een mogelijke ID Video-plugin. Wat zijn daarbij de randvoorwaarden? Denk daarbij aan de (infrastructurele) randvoorwaarden aan de gemeentekant. Maar ook aan de minimale uitgangspunten mbt jullie product, zoals aanwezige deelproducten/modules, softwarereleases etc. Hoe wordt ervoor gezorgd dat (bijzondere) persoonsgegevens zodanig worden verwerkt dat deze voldoen aan de eisen die eraan worden gesteld voor overheden?
    - Wat zijn de eenmalige kosten voor het daadwerkelijk bouwen van een plugin (waarbij de randvoorwaarden als een gegeven beschouwd mogen worden)?
    - Wat is een reële doorlooptijd voor het bouwen van een dergelijke plugin?
    - Geef een indicatie van jullie commerciëlere prijsvoering richting iedere organisatie die wil aansluiten obv jullie product.
